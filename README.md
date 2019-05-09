# just-a-card-hugo
A hugo theme that's just-a-card. Dead simple. Best for personal introduction page.

![just-a-card screenshot](https://github.com/achooan/just-a-card-hugo/blob/master/images/screenshot.png)

## Installation
If you have a hugo project already, then simply add it to your themes.
```
git init // skip this if you have initialized git.
git submodule add https://github.com/achooan/just-a-card-hugo themes/just-a-card

// In case you need to update the theme to the latest version, run this command.
git submodule update --rebase --remote
```

Else, you can just clone this theme to your project.
```
git clone https://github.com/achooan/just-a-card-hugo themes/just-a-card
```

## Configuration
To use this theme, configure `theme` in your `config.toml` file.
```
#config.toml
theme = "just-a-card"
```
Then, add the following lines to your `config.toml`
```
[author]
  name = "John Doe"
  title = "Software Engineer"
  location = "Somewhere in the world"
  company = "Company Inc."
  companyUrl = "#"
  intro = "Lorem ipsum dolor sit amet, ..."
  profile_image = "images/profile.jpeg"

[params]
  primary_color = "#ffe9a0"
  secondary_color = "#4789d8"
  google_font = "Overpass"

  [[params.links]]
    icon = "link"
    name = "E-mail"
    url = "mailto:#"
  [[params.links]]
    icon = "github"
    name = "Github"
    url = "https://github.com/#"
  [[params.links]]
    icon = "file-text"
    name = "Hire me!"
    url = "/pdf/#"
```

### Images
Include `profile` image inside `static/images` folder. It doesn't matter which image format you use, as long as you edit the `config.toml` accordingly.

### Colors
Any browser-recognizable colors are possible. (eg. #FFFFF, white, #DDD). `primary_color` is a color for the background (eg. yellow) and `secondary_color` is a color for the border and the footer (eg. blue).

### Font
This theme uses [Google Font](https://fonts.google.com). Simply add the font name to `google_font` (default font is `Overpass`).

### Icons
This theme uses UiKit Icons. Please refer to [UIKit Icons](https://getuikit.com/docs/icon)

### Links
You may add more links, but be sure to have a proper links. If you wish to add new link, then simple append this format:
```
[[params.links]]
  icon = 
  name = 
  url = 
```

## License
See [LICENSE](https://github.com/achooan/just-a-card-hugoblob/master/LICENSE)
