# Static HTML Generator

This is a simple HTML generator built with [Jinja2](https://github.com/pallets/jinja) and [Python-Markdown](https://github.com/Python-Markdown/markdown). I use it to power my blog. Most blog generators, like hexo, are too complex. I just want a simple one without too many useless functions.

## Requirements

```bash
pip install Jinja2
pip install markdown
pip install pymdown-extensions
```

---

## Dart-Generator

I first built this generator using Dart and Mustache, but the markdown library of Dart just supports the basic markdown syntax and Mustache is not powerful enough.

The code of Dart-Generator is in the branch [dart-gen](https://github.com/yangtau/static-blog-generator/tree/dart-gen).
