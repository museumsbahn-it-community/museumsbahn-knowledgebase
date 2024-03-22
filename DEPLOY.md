# Deployment

currently we deploy to github pages

## Installation

```
pip install mkdocs
pip install mkdocs-include-dir-to-nav
```

## Deploy

```
mkdocs gh-deploy

# unfortunately mkdocs deletes the cname file, so we have to add it manually again
git checkout gh-pages
echo "chaosbahn.eu" >> CNAME
git add CNAME
git commit -m "add CNAME file"
git push
```


