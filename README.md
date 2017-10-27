# Jekyll Photo Gallery

I want to share my jekyll photo gallery, simple, functional, mobile friendly and most essential, pretty! The gallery is based on the design from [Henrrique Gusso](https://gus.so/) and utilizes the [jekyll gallery generator plugin](https://github.com/ggreer/jekyll-gallery-generator) to do most of the heavy lifting (with some minor changes).

![Example Image](https://i.imgur.com/vpmSx7S.png "Optional title")

**DEMO GALLERY:**
https://www.danielandrade.net/photos/

## Dependencies
(copied from the plugin repo)

* [ImageMagick](http://www.imagemagick.org/)
* [RMagick](https://github.com/rmagick/rmagick)
* [exifr](https://github.com/remvee/exifr/)
* [Ruby](https://www.ruby-lang.org) >= 2.1

### Install dependencies on OS X

```bash
brew install imagemagick rbenv
rbenv install 2.4.0
rbenv global 2.4.0
gem install rmagick exifr
```

### Install dependencies on Ubuntu

```bash
apt install libmagick++-dev
gem install rmagick exifr
```

## Configuration

This plugin reads several config options from `_config.yml`. The following options are supported (default settings are shown):

```yaml    
# The following options are for individual galleries.
gallery:
  dir: photos               # root folder with all the pictures 
  title: "Photos"           
  sort_field: "date"        # sort pictures by date
  title_prefix: ""          # title prefix
  symlink: false            # false: copy images into _site. true: create symbolic links (saves disk space)
  thumbnail_size:           # 
    y: 450                  #
    retina: 1.5             #
  galleries:
    2017_Berlin:            # folder name
      name: "Berlin"        # gallery name
      date: "2017/08/01"    # gallery date
      best_image: 0062.jpg  # best photo for gallery blur image and gallery index 
```

## Thanks to
* The people behind jekyll projecy
* [Geoff Greer](https://github.com/ggreer) for the script
* [Gusso](https://github.com/gusso) for the design
