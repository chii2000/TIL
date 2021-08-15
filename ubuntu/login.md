# sshまで
raspberry pi imager でubuntu desktop 20.04を焼くとログインまで行かずに切れる。→balenaetcherで焼く。  
ログインできない。→新しいgigastoneの32GBのsdカードで焼き直し。→うまくいった。  
wifiのSSIDとパスワードをnetwork-configに書き換え  
ip addr するもipアドレスがない。→　sudo reboot
wlan0からのipアドレスをゲット
pcのコマンドラインでssh ubuntu@ipアドレス



