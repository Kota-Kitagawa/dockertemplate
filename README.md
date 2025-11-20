## 概要
ubuntuイメージを元にしたコンテナ  
https化するための自己証明書発行のため作成（自由に変更可）
## installされてるもの
- vim
- openssl

  ## ssl証明書作成コマンド
  ```
  openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout /etc/nginx/ssl/nginx.key -out /etc/nginx/ssl/nginx.crt -subj "/C=JP/ST=Tokyo/L=Tokyo/O=Localhost/OU=Development/CN=localhost"
  ```
