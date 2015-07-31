# coap-extension
Tizen Crosswalk extension for Iotivity

This projects provides a Tizen-Crosswalk extension for Iotivity


# Install
openssl genrsa -out tools/mykey.pem 1024
./make_xpk.sh app/ tools/mykey.pem xwalk-ioc-extension-demo

# Demo application
root# su - guest
guest# pkgcmd -i -t xpk -q -p xwalk-ioc-extension-demo.xpk
guest# ail_list
guest# xwalk-launcher xwalk.<appid>
```
To uninstall:
```shell
guest# pkgcmd -u -t xpk -q -n <appid>
```


