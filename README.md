## Configuring github action for publishing to github pages  

1. Generate key pair

```shell
ssh-keygen -t rsa -b 4096 -C "ilya.vlasov.inmost@yandex.ru" -f gh-pages -N ""
```

2. Put ```cat gh-pages.pub``` to GitHub repo -> settings -> deploy keys

3. Put ```cat gh-pages``` to GitHub repo -> settings -> secrets
