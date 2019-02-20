# Moodleをdockerで動かす  
## moodleのインストール手順
1. docker-composeでコンテナを立てる

1. 言語の選択  
    すきな言語を選択する    

1. パスの確認  
    デフォルトのままでOK  
    `/var/www/moodledata`  

1. データベースドライバを選択する  
    `improved MySQL`    

1. データベース設定  
    データベースホスト；`mdl_mysql5.6`  
    データベース名；`moodle`  
    データベースユーザー；`root`  
    データベースパスワード；`XXXX`  
    ※`MYSQL_ROOT_PASSWORD=XXXX`で設定したパス  
    テーブル接頭語；`mdl_`  
    データベースポート：　空欄  
    Unixソケット：　空欄  

