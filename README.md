![PineDocs](https://i.imgur.com/sNOMpuK.png)

PineDocs is a simple, fast, lightweight tool for viewing files in a browser. Great for documentation, wiki, notes, etc.

Renders Markdown, HTML, syntax highlighting code, images, GIFs, SVG, audio and small videos.

## Features
- Cross-platform (currently tested on Ubuntu and Windows).
- No database needed.
- Supports Markdown, text, HTML, images, GIFs, audio and videos.
- Syntax highlighting for over 169 languages with over 77 themes.
- Multiple responsive themes and color schemes.
- YAML Config file to change the settings.
- Quick filtering in files


## Setup
### Requirements
- PHP 7.0 or above
	- YAML extension for PHP (https://pecl.php.net/package/yaml)
- Web server: Apache2, nginx, etc.


### Setup guide
1. [Download the latest release](https://github.com/xy2z/PineDocs/releases) or `git clone`
1. Setup the web server to the /public dir (use `php -S localhost:89` for testing)


## Configuration
Feel free to edit the `config.yaml` file to fit your needs.


#### Settings
- **`title`**  (string) The title of the site, used in tabs and bookmarks.

- **`content_dir`** (string) Path to the dir you want to use. Default is the PineDocs/content/ dir.

- **`logo`** (string) Path to the logo. If nothing is set, the PineDocs logo will be used.

- **`index`** (string) Relative path to the index file. Default is array of `index.md`, `index.html`, `index.txt`, `index`.

- **`theme`** (string) Available themes: `default`, `default-dark`, `wiki`, `wiki-dark`.

- **`highlight_theme`** (string) The theme to use for code. See a list at https://highlightjs.org/static/demo/

- **`code_transparent_bg`** (bool) If `true`, all  will use the highlight theme. If `false`, the background will be transparent.

- **`open_dirs`** (int|string) The number of levels of dirs that should be opnened on page load. Use `all` to open all dirs.

- **`render_footer`** (bool) Render the menu footer?

- **`exclude_files`** (array) List of files to exclude. Supports regex if the format is /regex/i.

- **`show_file_extension`** (bool) Show file extensions. Default is true.


## License
GNU GPLv3. See LICENSE.txt
