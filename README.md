# Ubuntu-MATE-Keymap-for-Mac-Japanese-Keyboard

This is a key configuration files for using a Mac keyboard in Ubuntu MATE like macOS.

## How to install .Xmodmap

1. Click on the green “Code” button in the upper right corner of the repository's top page.

2. Select “Download ZIP” from the menu that appears.

3. Unzip the downloaded ZIP file.

4. Place “home_user_.Xmodmap” in “/home/*Your User Name*/” and remove “home_user_” from Rename.

5. Open a terminal, run “sudo apt update”, enter your password, and then run “sudo apt install x11-xserver-utils” to install Xmodmap on your Ubuntu MATE.

6. Execute “xmodmap ~/.Xmodmap” to reflect the key settings.

# How to Install the Mozc Keymap

*I am going to assume that your language setting is Japanese.

1. If you are in Mozc Input Mode, click to select an appropriate key input box, then press the 「あ」 (“A”) icon at the top right of the MATE desktop.

2. Open the 「Mozcツール」 (“Mozc Tools”) and select 「設定ツール」 (“Configuration Tool”).

3. From 「キー設定の選択」 (“Select Keymap”), choose 「編集...」 (“Edit...”)

4. From 「編集🔽」 (“Edit🔽”), select 「インポート...」 (“Import...”); after selecting “OK”, open “ubuntu_mozc_keymap_for_mackey.txt”.

5. Select “OK” and then “適用” (“Apply”).

After all steps are complete, save all important data and restart your Mac.

~

# Ubuntu MATEキーマップ（Mac日本語キーボード用）

これは、Ubuntu MATEでMacの日本語キーボードをmacOSのように使うためのキー設定ファイルです。

## .Xmodmapのインストール方法

1. このリポジトリ（Githubページ）のトップページ右上にある、緑色の「Code」ボタンをクリックします。

2. 表示されるメニューから「Download ZIP」を選択します。

3. ダウンロードされたZIPファイルを解凍してください。

4. 「home_user_.Xmodmap」を「/home/*Your User Name*/」に配置し、名前を変更から「home_user_」を削除します。

5. ターミナルを開き、「sudo apt update」を実行し、パスワードを入力したのち「sudo apt install x11-xserver-utils」を実行して、お使いのUbuntu MATEにXmodmapをインストールします。

6. 「xmodmap ~/.Xmodmap」を実行し、キー設定を反映させます。

## Mozcキーマップのインストール方法

1. Mozc入力モードになっている場合は、適当なキー入力ボックをクリックして選択し、MATEデスクトップの右上の「あ」を押してください。

2. 「Mozcツール」の「設定ツール」を開いてください。

3. 「キー設定の選択」から「編集...」を選んでください。

4. 「編集🔽」から「インポート...」を選び、「OK」を選んだのち、「ubuntu_mozc_keymap_for_mackey.txt」を開いてください。

5. 「OK」「適用」を選んでください。

すべての手順が終わったら、重要なデータをすべて保存したのち、Macを再起動してください。
