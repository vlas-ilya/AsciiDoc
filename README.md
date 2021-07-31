## AsciiDoc -> Github Actions -> Github Pages

Pipeline for Github Actions for building and publishing AsciiDoc into Github Pages

## Configuring github action for publishing to github pages  

1. Generate key pair

```shell
ssh-keygen -t rsa -b 4096 -C "<your email>" -f gh-pages -N ""
```

2. Put ```cat gh-pages.pub``` to GitHub repo -> settings -> deploy keys (any name, but set "Allow write access" checkbox)

3. Put ```cat gh-pages``` to GitHub repo -> settings -> secrets (with name ACTIONS_DEPLOY_KEY)

## Local building

1. Install https://asciidoctor.org/
2. Install https://asciidoxy.org/
3. Run ```asciidoxy --base-dir docs --destination-dir ./public --multipage ./docs/index.adoc```
4. Run ```cp -r ./docs/resources ./public/```
5. Result will store in ```public/index.html```

## Documentation

* https://asciidoc.org/
* https://asciidoxy.org/
