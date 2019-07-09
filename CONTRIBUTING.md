# Contributing to govips
First, thank you for supporting. I believe together we can make this one of the most useful Go libraries for image manipulation available.

## Have an issue, idea or question?
Please create a [new issue](https://github.com/davidbyttow/govips/issues/new) with as much information as possible.

If you're having installation problems, please include any and all output from your commandline.

## Want to write some code?
I'd love it for you to take initiative and submit pull requests. It's extra awesome if your code has unit tests to support the change. Let's do this together! I'll add you to the list of contributors.

## Strict linting
The Travis build currently checks strict format and linting, so be sure to add comments!

## Build

### On Mac
```bash
brew install pygobject3 gtk+3

virtualenv run
source run/bin/activate
pip install pycairo
pip install PyGObject
pip install pyvips

bash scripts/build.sh
```

### On Ubuntu/Debian
```bash
sudo apt install python3-gi python3-gi-cairo gir1.2-gtk-3.0

virtualenv run
source run/bin/activate
pip install pycairo
pip install PyGObject

```

## Run the tests

```sh
CGO_CFLAGS_ALLOW=-Xpreprocessor go test ./...
```

## Get in touch

Have a question not covered here? Feel free to email me at [david.byttow@gmail.com](mailto:david.byttow@gmail.com)
