## AsciiDoc -> Github Actions -> Github Pages

Pipeline for Github Actions for building and publishing AsciiDoc into Github Pages

## Configuring github action for publishing to github pages  

1. Generate key pair

```shell
ssh-keygen -t rsa -b 4096 -C "<your email>" -f gh-pages -N ""
```

2. Put ```cat gh-pages.pub``` to GitHub repo -> settings -> deploy keys

3. Put ```cat gh-pages``` to GitHub repo -> settings -> secrets

## Local building

1. Install https://asciidoctor.org/

2. Run ```asciidoctor -D public --backend=html5 -o index.html docs/index.adoc```

3. Result will store in ```public/index.html```

## Documentation

https://asciidoc.org/
