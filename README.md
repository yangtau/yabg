# Yet Another Blog Generator

*yabg* is a simple static blog generator built with [Jinja2](https://github.com/pallets/jinja) and [Python-Markdown](https://github.com/Python-Markdown/markdown).
I use it to power my blog. Most blog generators, like hexo, are too complex.
I just want a simple one without too many useless functions, so I build this one.

**example**: [yangtau.me](https://yangtau.me)

## Requirements

```bash
pip install Jinja2
pip install markdown
pip install pymdown-extensions
pip install PyYAML
```

## Config

- [ ] TODO

## Build

```bash
python3 yabg/main.py config.yaml
```

## [now.sh](https://now.sh) Deployment

```yaml
FRAMEWORK PRESET: other
BUILD COMMAND: pip install PyYAML Jinja2 markdown pymdown-extensions && python3 yabg/main.py
OUTPUT DICTORY: public # setted in your config.yaml
```

Add `rm -rf public/` if you need to clear the old one before building the new one (if your `output_dir` in config.yaml is `public/`):
```yaml
BUILD COMMAND: pip install PyYAML Jinja2 markdown pymdown-extensions && rm -rf public/ && python3 yabg/main.py
```


# Dart-Generator

I first built this generator using Dart and Mustache, but the markdown library of Dart just supports the basic markdown syntax and Mustache is not powerful enough.

The code of Dart-Generator is on the branch [dart-gen](https://github.com/yangtau/static-blog-generator/tree/dart-gen).
