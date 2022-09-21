# gif-for-ubuntu
Install gif reader

You download some gif file and you try to open with image viewer but something was wrong

## Try this simple way

### Update

```
sudo apt-get update -y  
```
### Install gifsicle

```
sudo apt-get install -y gifsicle
```

### Create desktop file (ex.gifsicle.desktop) and copy this and save it:

```bash
[Desktop Entry]
Name=GIFview 
Exec=gifview -a %f
Icon=gif
Terminal=false
Type=Application
StartupNotify=true
NoDisplay=true
MimeType=image/gif
```
### And put it into ~/.local/share/applications
```
mv ~/.local/share/applications ./gifsicle.desktop
```
