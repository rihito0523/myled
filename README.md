# ロボットシステム学課題１　LED点滅ギミック追加  
# 使用道具　　
・ラズベリーパイ４  
・LED（青）  
・ブレッドボード  
・抵抗  
・ジャンパー線  
# 使用方法  
## インストール  
ラズベリーパイ上で　git clone https://github.com/rihito0523/myled.git
myled,Makefileが同じディレクトリにインストールしてあることを確認し、ディレクトリ内でmake
同じファイル上にmyled.koができていれば準備完了。  
## 実行  
sudo insmod myled.ko  
sudo chmod 666 /dev/myled0  
上記を入力した後、下記の実行したいコマンドを入力する。  
echo 1 > dev/myled0　　点灯  
echo 2 > dev/myled0　　点滅  
echo 0 > dev/myled0　　消灯  
sudo rmmod myledで終了。  
