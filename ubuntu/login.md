# sshまで
raspberry pi imager でubuntu desktop 20.04を焼くとログインまで行かずに切れる。→balenaetcherで焼く。  
ログインできない。→新しいgigastoneの32GBのsdカードで焼き直し。→うまくいった。  
wifiのSSIDとパスワードをnetwork-configに書き換え  
ip addr するもipアドレスがない。→　sudo reboot
wlan0からのipアドレスをゲット
pcのコマンドラインでssh ubuntu@ipアドレス


# ipアドレスの固定化
/etc/netplan/
cp 50-cloud-init.yaml .bak yanlのコピー
vi 50-cloud-init.yaml で編集  
address　サブネット 32bit*3 /24 ネットマスク
gateway 中継役
nameserver　複数設定できる　変換役


