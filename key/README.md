```shell
openssl genrsa -out server.key 2048
openssl req -new -key server.key -out server.csr

openssl x509 -signkey server.key -in server.csr -req -days 365 -out certificate.crt

openssl pkcs12 -export -out windows-signing.pfx -inkey server.key -in certificate.crt


openssl pkcs12 -export -out windows-signing.pfx -inkey private.key -in certificate.crt
```

```shell
set CLITEST_WINDOWS_SIGNING_PASS=123456789 && oclif pack win --root=.
set NODE_ENV=production && set WINDOWS_SIGNING_PASS=123456789 && oclif pack win --root=.
set NODE_ENV=production && set CLITEST_WINDOWS_SIGNING_PASS=123456789 && oclif pack win --root=.
set DEBUG=* && set CLITEST_WINDOWS_SIGNING_PASS=123456789 && oclif pack win --root=.
set NODE_ENV=production && set OCLIF_WINDOWS_SIGNING_PASS=123456789 && npx oclif pack win --root=.
set NODE_ENV=production && set OCLIF_WINDOWS_SIGNING_PASS=123456789 && oclif pack win --root=.
```
