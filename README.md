# test-tcp
受信する側、ホストサーバーはファイアウォールの設定を変えてください。

ターミナルより
#ufwのダウンロード
sudo apt update
sudo apt install ufw
#ufwの停止
sudo ufw disable
#ssh,8080/tcp,vncポートの開放
sudo ufw allow 8080/tcp
sudo ufw allow ssh
sudo ufw allow 5900/tcp
#ufw再起動
sudo ufw enable
#ufwの確認
sudo ufw status
#ポートの確認
sudo netstat -tlnp
