![Preview](/_github/screen.png)

config.json:
```json
{
  "settings": {
    "workPath": "./",
    "outPath": "../res/",
    "tinyKey": "your api key"
  },
  "atlases": {
    "ui": {
      "images": {
        "exclude": "timer",
        "templates": ["**/*.png"]
      },
      "work": "textures/ui/",
      "tpOptions": {
        "--opt": "RGBA5555"
      },
      "fonts": [
        {
          "dense": true,
          "path":"fonts/Tahoma14",
          "name":"Tahoma14"
        },
        {
          "dense": true,
          "path":"fonts/ScoreNums",
          "name":"ScoreNums"
        }
      ],
      "tinify": true,
      "out":"ui/"
    },
    "flanim": {
      "name": "FlashAnimation",
      "keyPath": "anim/flash/",
      "work": "textures/animation/flash",
      "tpOptions": {
        "--opt": "RGBA5555"
      },
      "tinify": true,
      "out":"anim/"
    }
  }
}
```

Run:
```bash
python Content.py
# or
python Content.py -p flanim
# or
python Content.py -p ui flanim
# or
python Content.py -c MyConfig.json -p ...
```