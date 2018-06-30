## linux  启动 ssr 时报错 `undefined symbol: EVP_CIPHER_CTX_cleanup`

1. 打开 `shadowsocksr/shadowsocks/crypto/openssl.py` 
2. 将第 52 行和第 111 行的 `cleanup` 改为 `reset` 
3. 保存并退出

之后启动 ssr 就不会报错了。
