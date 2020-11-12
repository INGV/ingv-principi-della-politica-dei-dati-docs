|**Service**|**Master**|**Develop**|
|---|---|---|
|CircleCI|[![CircleCI](https://circleci.com/gh/INGV/ingv-principi-della-politica-dei-dati-docs/tree/master.svg?style=svg)](https://circleci.com/gh/INGV/ingv-principi-della-politica-dei-dati-docs/tree/master)|[![CircleCI](https://circleci.com/gh/INGV/ingv-principi-della-politica-dei-dati-docs/tree/develop.svg?style=svg)](https://circleci.com/gh/INGV/ingv-principi-della-politica-dei-dati-docs/tree/develop)|

# ingv-principi-della-politica-dei-dati-docs

Maggiori info sul concetto adottato per la generazione di questa documentazione:
- https://github.com/INGV/test-docs-italia

## Debug sul proprio PC
```
$ docker run -it -v /tmp/temp_dir:/tmp/temp_dir --rm python:3.7 bash
. . .
#
# apt-get update && apt-get install -y texlive-base texlive-latex-base texlive-latex-recommended texlive-fonts-recommended texlive-fonts-extra texlive-latex-extra texlive-formats-extra texlive-bibtex-extra texlive-humanities texlive-lang-italian texinfo texlive-science latexmk vim
. . .
#
# mkdir -p /root/project
# cd /root/project/
~/project#
~/project# git clone https://github.com/INGV/ingv-principi-della-politica-dei-dati-docs.git
. . .
~/project# cd ingv-principi-della-politica-dei-dati-docs
~/project/ingv-principi-della-politica-dei-dati-docs# git submodule update --init --force
. . .
~/project/ingv-principi-della-politica-dei-dati-docs# pip install -r requirements.txt
. . .
~/project/ingv-principi-della-politica-dei-dati-docs# make html
. . .
~/project/ingv-principi-della-politica-dei-dati-docs# cp -R _build/html /tmp/temp_dir/
```

## Guide
### Configurazione CircleCI + GitHub Pages
- https://circleci.com/blog/deploying-documentation-to-github-pages-with-continuous-integration/

### Sphinx:
- https://www.sphinx-doc.org/en/master/usage/configuration.html

## Sito GitHub Page
- https://ingv.github.io/ingv-principi-della-politica-dei-dati-docs/
