
Prepare USB:
```
Disk Utility - Erase:
    Name: macos12
    Format: Mac OS Extended (Journaled)
```

Prepare SSD:

```
Input Recovery (press and hold touch button)

Options - Disk Utility - Erase
    Name: macos
    Format: APFS
    Erase Volume Group «Стереть группу томов»
```


Make USB macos:

```
Download the macOS Monterey Installer from AppStore

System Settings > Security & Privacy > Full Disk Access-> Terminal: ON

open Terminal.app:
    sudo /Applications/Install\ macOS\ Monterey.app/Contents/Resources/createinstallmedia --volume /Volumes/macos12 --nointeraction
```

