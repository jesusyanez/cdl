# LootDL

<img src="https://github.com/jesusyanez/example-images/blob/main/downloader-example.gif?raw=true" />

Downloader for Google Drive, Dropbox, Mediafire, and WeTransfer.

- Python 3 
- Works on all operating systems
- No API keys / credentials needed
- Auto extracts .zip files
- Auto extracts .rar files (requires 7zip)
- Auto deletes compressed files after extraction



## Usage
```python3
import lootdl

# lootdl.grab(url, downloads folder path)
lootdl.grab('https://drive.google.com/file/d/.../view?usp=sharing', './Downloads/')
```

### Bulk Usage
```python3
import lootdl

download_list = ['URL1', 'URL2', 'URL3']

for url in download_list:
 lootdl.grab(url, './')
```
Ensure the download location exists and ends with a "/" or it may cause issues. <br/>
You can use "./" to download to the folder LootDL is in.

## Supported URLs

Google Drive
```txt
https://drive.google.com/drive/folders/...?usp=sharing
https://drive.google.com/file/d/.../view?usp=sharing
```
Dropbox
```txt
https://www.dropbox.com/s/.../...?dl=0
https://www.dropbox.com/s/.../...?dl=1
https://www.dropbox.com/sh/.../...?dl=0
https://www.dropbox.com/sh/.../...?dl=1
```
MediaFire
```txt
https://www.mediafire.com/file/.../.../file
```
WeTransfer
```txt
https://wetransfer.com/downloads/.../...
```


## Roadmap
- [X] Google Drive
- [X] Dropbox
- [X] MediaFire
- [X] WeTransfer
- [ ] Mega
 
 ## Acknowledgements 
 
Thank you to the authors of the following repos:
- "gdrivedl" by matthuisman - https://github.com/matthuisman/gdrivedl
- "mediafire-dl" by Juvenal-Yescas - https://github.com/Juvenal-Yescas/mediafire-dl
- "transferwee" by iamleot - https://github.com/iamleot/transferwee
