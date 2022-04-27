# go-mtls

## Commands
### Start server
```shell
go run -v server.go
```
### Start client
```shell
go run -v client.go
```
### Generate certificate
```shell
openssl req -newkey rsa:2048 \
  -new -nodes -x509 \
  -days 3650 \
  -out cert.pem \
  -keyout key.pem \
  -subj "/C=BR/ST=Sao Paulo/L=Sao Paulo/O=Your Organization/OU=Your Unit/CN=localhost"
  ```
### Add Go Debug
```shell
echo 'export GODEBUG=x509ignoreCN=0' >> ~/.zshrc
```
