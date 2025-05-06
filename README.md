# Ubuntu-MATE-Keymap-for-Mac-Japanese-Keyboard

This is a key configuration file for using a Mac Japanese keyboard in Ubuntu MATE like macOS.

## Disclaimer

Tsuikyu assumes no responsibility whatsoever for the installation or use of this software on your computer.

## How to Install .Xmodmap

1. Click the green **"Code"** button at the top right of the repository's main page.
2. Select **"Download ZIP"** from the menu.
3. Unzip the downloaded ZIP file.
4. Place the file named `home_user_.Xmodmap` into your home directory (e.g. `/home/YourUserName/`) and rename it to `.Xmodmap` (remove `home_user_`).
5. Open a terminal and run:
    ```
    sudo apt update
    sudo apt install x11-xserver-utils
    ```
6. To apply the key settings, run:
    ```
    xmodmap ~/.Xmodmap
    ```

## How to Install the Mozc Keymap

*Assuming your language setting is Japanese.*

1. If you are in Mozc Input Mode, click to select an appropriate key input box, then press the 「あ」 (“A”) icon at the top right of the MATE desktop.
2. Open 「Mozcツール」 (“Mozc Tools”) and select 「設定ツール」 (“Configuration Tool”).
3. From 「キー設定の選択」 (“Select Keymap”), choose 「編集...」 (“Edit...”).
4. From 「編集🔽」 (“Edit🔽”), select 「インポート...」 (“Import...”); after selecting “OK”, open `ubuntu_mozc_keymap_for_mackey.txt`.
5. Select “OK” and then “適用” (“Apply”).
6. After all steps are complete, save your important data and restart your Mac to activate the new settings.

## Copyright

I waive copyright on the portions I have been involved in.

---

# Ubuntu MATEキーマップ（Mac日本語キーボード用）

これは、Ubuntu MATEでMacの日本語キーボードをmacOSのように使うためのキー設定ファイルです。

## 免責事項

これをあなたのコンピュータにインストールまたは使用したことによる一切の責任を、Tsuikyuは負いません。

## .Xmodmapのインストール方法

1. このリポジトリ（GitHubページ）のトップページ右上にある、緑色の**「Code」**ボタンをクリックします。
2. 表示されるメニューから**「Download ZIP」**を選択します。
3. ダウンロードされたZIPファイルを解凍してください。
4. `home_user_.Xmodmap` をホームディレクトリ（例: `/home/あなたのユーザー名/`）に配置し、「home_user_」を削除して `.Xmodmap` にリネームしてください。
5. ターミナルを開き、以下を実行します。
    ```
    sudo apt update
    sudo apt install x11-xserver-utils
    ```
6. キー設定を反映させるには、以下を実行します。
    ```
    xmodmap ~/.Xmodmap
    ```

## Mozcキーマップのインストール方法

*言語設定が日本語の場合を想定しています。*

1. Mozc入力モードになっている場合は、適当なキー入力ボックスをクリックして選択し、MATEデスクトップの右上の「あ」アイコンを押してください。
2. 「Mozcツール」から「設定ツール」を開いてください。
3. 「キー設定の選択」から「編集...」を選択してください。
4. 「編集🔽」から「インポート...」を選び、「OK」を押した後、`ubuntu_mozc_keymap_for_mackey.txt` を開いてください。
5. 「OK」「適用」を選択してください。
6. すべての手順が終わったら、重要なデータを保存し、設定を有効にするためMacを再起動してください。

## 著作権

私が関与した部分については著作権を放棄します。
