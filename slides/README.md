# Slides de la formation Python LBN

**Installez [reveal-md](https://github.com/webpro/reveal-md):**

```shell
npm install -g reveal-md
```

**Lien http vers le site contenant les exercices:**

```shell
export EXERCICE_URL=http://127.0.0.1:8080
```

**Pour visualiser les slides:**

```shell
reveal-md public/slides.md \
  --css public/style.css \
  --template public/reveal-template.html \
  --preprocessor public/preproc.js
```

**Pour exporter les slides au format static:**

```shell
reveal-md public/slides.md \
  --css public/style.css \
  --template public/reveal-template.html \
  --preprocessor public/preproc.js \
  --static _site
```

> Le site static sera situé dans le répertoire _site/
