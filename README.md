# Trisophic Union Documents

These are the core documents of the Trisophic Union defining how we organize.


Currently the constituon is signed using RSA keys.


The Constitution can be signed like this:



```
cat Constitution.md | ssh-keygen -Y sign -n file -f ~/.ssh/id_rsa > Constitution.sig
```


or verified


```
cat Constitution.md | ssh-keygen -Y check-novalidate -n file -f ~/.ssh/id_rsa.pub -s Constitution.sig
```
