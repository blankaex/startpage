# Startpage

Based on [startpage by fuyuneko](https://github.com/fuyuneko/startpage) *I think* (I can't actually remember where I stole it from).

![example screenshot (150418)](https://i.imgur.com/rcE2iob.jpg)
![example screenshot expanded (150418)](https://i.imgur.com/Qtz5p2O.jpg)

### Usage
The easiest way to make changes is by editing __config.json__ and __index.html__.

### JSON
| attribute    | if true                                              |
| ------------ | :--------------------------------------------------- |
| borders      | enables borders on top and bottom                    |
| alwaysopen   | makes all squares open on load                       |
| mascot       | enables image in the bottom right hand corner        |

The other attributes should explain themselves.

### HTML
To add/remove a square just add/remove a `div sqr` within `div cell`.
Keep the structure like this:
```
<div class="sqr">
    <span>HEADING</span>
    <div class="content">
        <a href="URL">LINK TITLE</a><br>
        <a href="URL">LINK TITLE</a><br>
        ...
        <a href="URL">LINK TITLE</a>
    </div>
</div>
```
### Advanced Search
The default search engine is **Google**, but flags can be prepended to the search query.
```
-g      gelbooru
-y      YouTube
-n      nico nico douga
-p      pixiv
```
`-p kneesocks` would search for **kneesocks** on **Pixiv**.
For gelbooru, use underscores `_` for tags with more than one word and separate multiple tags with spaces (e.g.: `thighhighs_pull 1girl`).