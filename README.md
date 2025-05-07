# Ubuntu MATEキーマップ（Mac日本語キーボード用）

これは、Ubuntu MATEでMacの日本語キーボードをmacOSのように使うためのキー設定ファイルです。

## 免責事項

これをあなたのコンピュータにインストールまたは使用したことによる一切の責任を、Tsuikyuは負いません。

## 説明

このキーマップは、以下のように反映されます。

- 「左コマンド（⌘）」が、「左Ctrl」になります。
- 「Control（^）」が、「Right Ctrl」になります。
- 「英数」が、「Eisu (Mozc)」になります。
- 「かな」が、「Hiragana (Mozc)」になります。

## キーボードモデルの設定方法

- セットアップ時に `sudo dpkg-reconfigure keyboard-configuration` を実行し、キーボードモデルに **Apple Aluminium (JIS)** を選択してください。
- 「英数」「かな」キーが期待通りに動作しない場合は、**Xorg**セッションでUbuntu MATEを起動しているか確認してください。
- キー割り当ての確認には、ターミナルで `xev` を使うと便利です。

## IBus Mozc（日本語入力）のインストール方法

1. ターミナルを開き、以下を実行します。
    ```
    sudo apt update
    sudo apt install ibus-mozc
    ```
2. インストール後、重要なデータを保存した後で、システムを再起動します。
    ```
    sudo reboot
    ```
3. 再起動後、「設定」アプリの「地域と言語」や「入力ソースの管理」から「日本語（Mozc）」を追加します。
4. 入力メソッドフレームワークが**IBus**になっていることを確認してください（「言語サポート」や「入力メソッド」設定で確認できます）。
5. 必要に応じて「日本語（Mozc）」をデフォルトの入力ソースに設定してください。

*これで、割り当てたキーで英語・日本語入力を切り替えられるようになります。*

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

## IBus Mozcキーマップのインストール方法

*言語設定が日本語の場合を想定しています。*

1. Mozc入力モードになっている場合は、適当なキー入力ボックスをクリックして選択し、MATEデスクトップの右上の「あ」アイコンを押してください。
2. 「Mozcツール」から「設定ツール」を開いてください。
3. 「キー設定の選択」から「編集...」を選択してください。
4. 「編集🔽」から「インポート...」を選び、「OK」を押した後、`ubuntu_mozc_keymap_for_mackey.txt` を開いてください。
5. 「OK」「適用」を選択してください。

すべての手順が終わったら、重要なデータを保存し、設定を有効にするためMacを再起動してください。

## 動作確認済み環境

MacBook Pro 15-inch Mid 2010 (SSD 512GB換装済み)  
Ubuntu MATE 20.04.5 Desktop (AMD64)

## 著作権

私が関与した部分については著作権を放棄します。

ただし、XmodmapはMITライセンス、MozcはBSDライセンスとなっていることにご注意ください。

## 最終更新

2025年5月7日 (JST)

## レコメンド

https://rapt-plusalpha.com

---

# Ubuntu-MATE-Keymap-for-Mac-Japanese-Keyboard

This is a key configuration file for using a Mac Japanese keyboard in Ubuntu MATE, making it behave like macOS.

## Disclaimer

Tsuikyu assumes no responsibility whatsoever for the installation or use of these files on your computer.

## Description

This keymap makes the following changes:

- “Left Command (⌘)” becomes “Left Ctrl”.
- “Control (^)” becomes “Right Ctrl”.
- “英数” becomes “Eisu (Mozc)”.
- “かな” becomes “Hiragana (Mozc)”.

## How to Configure Keyboard Model

- Run `sudo dpkg-reconfigure keyboard-configuration` during setup and select **Apple Aluminium (JIS)** for the keyboard model.
- If the “英数” and “かな” keys do not work as expected, make sure you are running Ubuntu MATE in a **Xorg** session.
- To check the key assignments, it is convenient to use `xev` in a terminal.

## How to Install IBus Mozc (Japanese Input)

1. Open a terminal and run:
    ```
    sudo apt update
    sudo apt install ibus-mozc
    ```
2. After installation, reboot the system after saving important data:
    ```
    sudo reboot
    ```
3. Once restarted, open the **Settings** app and go to **Region & Language**.
4. Click **Manage Installed Languages** or **Input Sources**, then add **Japanese (Mozc)** as an input source.
5. Make sure **IBus** is selected as your input method framework (you can check this in Language Support or Input Method settings).
6. Set **Japanese (Mozc)** as the default input method if needed.

*Now you should be able to switch between English and Japanese input using the assigned keys.*

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

## How to Install the IBus Mozc Keymap

*Assuming your language setting is Japanese.*

1. If you are in Mozc Input Mode, click to select an appropriate key input box, then press the 「あ」 (“A”) icon at the top right of the MATE desktop.
2. Open 「Mozcツール」 (“Mozc Tools”) and select 「設定ツール」 (“Configuration Tool”).
3. From 「キー設定の選択」 (“Select Keymap”), choose 「編集...」 (“Edit...”).
4. From 「編集🔽」 (“Edit🔽”), select 「インポート...」 (“Import...”); after selecting “OK”, open `ubuntu_mozc_keymap_for_mackey.txt`.
5. Select “OK” and then “適用” (“Apply”).

After all steps are complete, save your important data and restart your Mac to activate the new settings.

## Computers verified to work

MacBook Pro 15-inch Mid 2010 (SSD 512GB Installed)  
Ubuntu MATE 20.04.5 Desktop (AMD64)

## Copyright

I waive copyright on the portions I have been involved in.

Please note, however, that Xmodmap is under the MIT license and Mozc is under the BSD license.

## Last updated

May 7, 2025 (JST)

## Recommend

https://rapt-plusalpha.com