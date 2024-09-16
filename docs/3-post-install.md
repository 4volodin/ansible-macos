- [SystemPreferences](#systempreferences)
- [Build-in Apps](#build-in-apps)
    - [Dictionary](#dictionary)
    - [TimeMachine \& backup IOS:](#timemachine--backup-ios)
    - [Applications/Shortcuts:](#applicationsshortcuts)
    - [Safari](#safari)
      - [Toggl Track](#toggl-track)
- [Apps Downloaded from AppStore](#apps-downloaded-from-appstore)
    - [Things3 (licensed)](#things3-licensed)
    - [Mate (licensed)](#mate-licensed)
    - [StrongBox (licensed)](#strongbox-licensed)
    - [Amphetamine](#amphetamine)
    - [Mutekey](#mutekey)
    - [Hidden Bar](#hidden-bar)
    - [New File Menu](#new-file-menu)
    - [SessionRestore](#sessionrestore)
    - [install for iPad](#install-for-ipad)
- [Apps Downloaded using Brew](#apps-downloaded-using-brew)
    - [Little Snitch (licensed)](#little-snitch-licensed)
    - [Paw (licensed)](#paw-licensed)
    - [Dash (licensed)](#dash-licensed)
    - [Raycast](#raycast)
    - [Karabiner](#karabiner)
    - [ShoweEdge](#showeedge)
    - [Quitter](#quitter)
    - [XnView](#xnview)
    - [SSSReporter](#sssreporter)
  - [Stats](#stats)
    - [Firefox](#firefox)
    - [Acrobat Reader](#acrobat-reader)
    - [Evernote](#evernote)
    - [Telegram](#telegram)
    - [VLC](#vlc)
    - [Docker](#docker)
- [UNPAID](#unpaid)
    - [Valentina Studio](#valentina-studio)
    - [Multitouch:](#multitouch)
    - [PopClip](#popclip)
    - [Contexts](#contexts)
- [Only Rosetta](#only-rosetta)
    - [Winbox](#winbox)
- [Check list](#check-list)

---

yubi manager

Applications - OTP - slot 1 - challenge-response - insert secret key and Require touch: ON

---

    iMessage:
        - sync iCloud for iMessages
        - sync contacts on iCloud
        - on iPhone - Settings - Messages - Text Message Forwarding:  activate message forwarding to new Mac
    Apple Mail:
        - set up all email accounts
        - show most recent message at top
    Notes - Preferences:
        New notes start with: Body

    About this mac - Storage - Manage:
        Recomendations:
            Store in iCloud : ON
            Optimize Storage : OFF
            Empty Trash Automatically : ON

## SystemPreferences
    Wifi: Ask to join hotspots: ON
    Bluetooth - connect TrackPad, Keyboard
    Network:
        Firewall
            Turn on : ON
            Firewall options
                Control Centre.app Block incoming connections
                Universal Control.app Block incoming connections

    Notifications:
        Disable all without Calendar
    Sound:
        PlaySound on startup : OFF
    Focus:
    Screen Time:

    General:
        Software Update: Advanced: Download updates auto : OFF
        Sharing - disable all services
        Login Items:
            mountnas.sh
            Contexts, Popclip, Quitter, ShowyEdge, StrongBox
    Accessibility:
        Display:
            Display:
                Reduce motion : ON
                Reduce transparency : ON
            Pointer:
                increse Cursor size to second Position
        Spoken Content:
            System Voice : Siri (voice 1)
            Speak selection : ON
                Click i - and set Keyboard shortcut - LOOK at the hotkeys.md
                Use without modifier key
        PointerControl:
            TrackPad Options:
                Enable dragging: three finder drag
                Scrolling speed: 6/8
        Siri:
            Enable Type to Siri: ON
    Control Center:
        Wi-Fi: Show in Menu Bar: ON
        Battery:
            Show in Menu Bar : OFF
            Show Percentage : ON
            Show in Control Center: ON
        Other Modules: 
            Fast User switching:
                Show in Menu Bar: OFF 
        Menu Bar only:
            Clock:
                Date Options: Show date: ALWAYS
                Show day of the week: OFF
                Style: Digital
                Show AM/PM: OFF
            Spotlight: Show in menu bar : OFF
            Siri: Show Siri in menu bar : OFF
            Time Machine: Show in Menu Bar: ON
            VPN: Show in Menu Bar: ON

    Siri & Spotlight:
        Listen for "Hey Siri" : OFF
    Privacy & Security:
        Analytics & Improvements > uncheck all
        Apple Advertising > uncheck all
        Location Services:
            - Find My
            - Siri
            - Weather
            - Voice Memos
            - Reminders
            - Calendar
            - Wallet
        Accessibility:
            - Contexts
            - Dash
            - iTerm
            - Multitouch
            - PopClip
            - PuntoSwitcher
            - skhd
            - yabai
        Input Monitoring: ON
            - karabiner_grabber
            - karabiner_observer
            - Karabiner-EventViewer
            - Yubikey Manager
        Full Disk Access: ON
            - AppCleaner (for detail searching)
            - SuperDuper
            - Terminal
            - Alacritty
        Automation:
            iTerm.app:
                System Events.app (for using command 'theme' changing light-dark)
            Raycast.app:
                Amphetamine.app (for enable using )

    Desktop & Dock:
        Position on Screen: Left
    Displays:
        Night Shift: Sunset to Sunrise

    TouchID & Password:
        - LIndex, RMiddle, RRing
        - Enable all
     
    TrackPad:
        Point & Click:
            Look up & data detectors: Tap with three fingers
        Scroll & Zoom:
            Smart zoom  : OFF     (cancel delay when tap 2fingers)
        Point & Click:
            Tracking Speed: 9/10

    Keyboard:
        Keyboard Shortcuts:
            Display:
                Decrease brightness F14 : OFF
                Increase brightness F15 : OFF
            - MissionControl
                 Show NotificationCenter: Opt+[
                 Turn DND:                Opt+]
                 Switch Desktop:          1...7 Ctrl+ 1..7
                 Show Desktop:            press twice left control - keypad_1 from karabiner
            - Input Sources-> uncheck all
            - Spotlight:
                Show Spotlight search : ON (option + cmd + Space)
            - Services
                Translate with Mate         press left option twice - F18 from karabiner
                 Mic-onOff                  press right command twice - F ????????????????
        Text Input: Input Sources: Edit:
            Show Input menu in menu bar : Off
            Use the Caps Lock key to switch to and from ABC : Off
        Dictation:
            Dictation: On
            Shortcut: Press Left Command twice
            Language: Eng + Russian
                Customize Russian lang

    GPG Suite - Store in macOS Keychain: ON

## Build-in Apps

#### Dictionary

    Open Dictionary-Preferences and set
    -   New Oxford American Dictionary (English US)
    -   Oxford Russian Dictionary (Russian-English)
    -   Oxford American Thesaurus
    -   Толковый словарь русского языка (Russian)

#### TimeMachine & backup IOS:

_TimeMachine:_

    /usr/bin/osascript -e 'mount volume "smb://voale@10.100.1.2/timemachine"'

    # подключить диск timemachine в Preferences-TimeMachine
    tmutil destinationinfo

    SystemPreferences - Time Machine:
        Select Disk:
            timemachine on "10.100.1.2"
            Encrypt Backup Disk: ON
        Back Up Automatically: OFF
        Show Time Machine in menu bar: OFF

    Settings-> Spotlight-> Privacy->Add Network disks to prevent Spotlight from searching these locations
    //nas.home.lan/...
    //nas.home.lan/timemachine

    mdutil -i off /Volumes/timemachine
    mdutil -s /Volumes/timemachine

_Backup IOS:_

    /usr/bin/osascript -e 'mount volume "smb://voale@nas.home.lan/ios-backup"'

    SystemPreferences - Security & Privacy - Privacy:
      Full Disk Access:
        Terminal: ON

    ln -s /Volumes/ios-backup/voale ~/Library/Application\ Support/MobileSync

#### Applications/Shortcuts:

        Preferences - Sidebar:
            Quick Actions: OFF
            Menu Bar: OFF

#### Safari

    Menu - View:
        Show Status Bar : ON
        Show favorites bar : ON
    Preferences:
        Advanced:
            Show Develop menu in menu bar : ON
            Show full website address: ON
            Press Tab to highlight each item on a web page: ON
        Websites:
            Notifications:
                Allow websites to ask for permission to send notification: OFF

##### Toggl Track

    Settings:
        General:
            Show timer in menu bar: ON
        Shortcuts:
            Show/hide Toggl Track : Hyper+by
            Focus app when : timer stops

## Apps Downloaded from AppStore

#### Things3 (licensed)

    Open Things3 - Preferences - Things Cloud - Quick Entry:
        quick entry: Hyper+b

????? set ctrl-opt+space - quick entry with autofill

#### Mate (licensed)

    Mate - Already subscribed? - Login
    Preferences Mate
    Global shortcut and press cmd+opt+ctrl+shift+c => set hyper+cmd+c
    Translate clipboard by shortcut : ON
    Autoclear previous result : ON

#### StrongBox (licensed)

    defaults export com.markmcguill.strongbox filepath/filename


    SystemPreferences - Extensions - Added Extensions
        - Strongbox
            Password Autofill : ON
    StrongBox - menu bar - Upgrade to Pro - Restore previous purchase

    StrongBox - Preferences
        - General
            - Auto Lock Database after 60 sec : On
        - Password Generation
                Algorithm : Diceware
                count : 4
                Casing : Lowercase
                Word Lists Harry Potter EFF Fandom
        - Advanced
            - Hide Key file Name on Lock Screen : ON
            - Colorize Passwords : OFF
        - Autofill
            - enable Autofill for Database : On
            - use Wormhole fill if unlocked : On
            - enable quicktype : On

    StrongBox -> Add Database -> iCloud/Strongbox/troyan

#### Amphetamine

    Preferences:
        General:
            Launch Amphetamine at login: ON
        Triggers:
            - Name:MyiPhone
            - Wi-Fi Network:iPhone
            - Allow display to sleep: ON
        Appearance:
            Menu bar image: Owl
            Use low opacity when inactive: OFF

#### Mutekey

    Preferences
        - Launch at Login
        - open Desktop and press twice Fn to setup F17 hotkey

#### Hidden Bar

    Preferences
        Start Hidden Bar when login in : ON
        Show preferences on launch : OFF

#### New File Menu

    SystemPreferences - Added Extensions - New File Menu
        Finder Extensions : On

    Preferences
        - General
            Show file on creation finish: On
            Do not ask for filename: Off
            Show in menu bar : Off

#### Just Focus

    Preferences:
        General:
            Launch at login: ON
        Screen:
            Use the desktop picture: ON
            Quotes: None

#### SessionRestore

    Preferences - General:
            Sync Settings and Saved Sessions : On

#### install for iPad

    Yandex.Translate
    Билайн тв
    Reword English Language Learning App

## Apps Downloaded using Brew

#### Little Snitch (licensed)

    Preferences:
        Alert:
            Detail Level : Show port and Protocol Details
            Rule Lifetime: for 1 Minute
        APS:
            Enable autoatic profile switching: on

        Fil - New Profile:
            ⚠️ Office
            ✅Home- Active
            ❗️Public

#### Paw (licensed)

    Preferences - Paw Cloud - login on paw.cloud

#### Dash (licensed)

    Preferences - General:
        Syncing - SetUp Syncing - Set Sync Folder: ~/iCloud Drive/dev/dash
        Enable all checkboxes

#### Raycast

    Preferences:
        General:
            Startup:
                Launch Raycast at login: ON
            Raycast Hotkey: Opt+Space
            Show Raycast in menu bar: OFF
            Window mode: Compact
        Advanced:
            Navigation Bindings: Vim Style
        Extensions:
            Clipboard History: OFF
            Developer: OFF
            File Search: OFF
            Floating Notes: OFF
            Navigation: OFF
            Quicklinks: OFF
            Raycast:
                Changelog: ON
                Check For Extensions Updates: ON
                Check For Updates: ON
            Raycast Preferences: OFF
            Raycast for Teams: OFF
            Raycast for Teams: OFF
            Shortcuts: OFF
            Snippets: OFF
            Things:
                Show Today in Menu Bar: OFF
            Window Management: OFF
            
            Scripts:
                Script commands - Add directories - ~/bin

    install
        Amphetamine: ON
        Connect to VPN: ON
        Dash: ON
        Kill process: ON
        Port Manager: ON
        tldr: ON
        Things3: ON
        Toggl Track: ON
        Wi-Fi: ON
        Word Search: ON
        Toothpick: ON
    maybe:
        Can I Use: ON
        Color Casket: ON
        Lorem Ipsum: ON
#### Karabiner

    Karabiner:
        Misc:
            Show icon in menu bar: OFF
            Show profile name in menu bar: OFF
        Devices:
            enable Yubikey OTP+FIDO+CCID

#### ShoweEdge

    Preferences - Basic:
        Open at login : ON
        Show icon in menu bar : OFF
        ABC - blue color
        Russian - red color
        Indicator - Height - 3.45

#### Quitter

    Start quitter at login
    Edit Rules: [ "Activity Monitor", "Amphetamine", "App Store", "AppCleaner", "Books", "Calendar", "Contacts", "Dictionary", "Disk Utility", "FaceTime", "Find My", "Hand Mirror", "Karabiner-Elements", "Karabiner-EventViewer", "Keychain Access", "LaunchControl", "Little Snitch", "Mail", "Maps", "Messages", "Music", "News", "Photos", "Podcasts", "Preview", "Reminders", "Shortcuts", "Skype", "SystemSettings", "Telegram"]

#### XnView

    Preferences-> Inteface-> Keyboard-> Space - Next file

#### SSSReporter

    Launch SSDReporter at login : On
    Display in Menubar instead of the Dock : On
    Settings - Appearance - Display App-Icon: Nowhere

#### Firefox

    Preferences
        Startup:
            Open previous windows and tabs : ON
    Install Extensions: FoxyProxy, VPNLY
    FoxyProxy:
        Aeza squid 3128:
            proxy type: http
            proxy ip: 10.0.1.101
            port: 3128
            username: voaleproxy
            passs: ...
        Aeza ssh -D :9050:
            proxy type: socks5
            proxy ip: 127.0.0.1
            port: 9050
            username: 
            passs: 
        Aeza Dante :1080    
            proxy type: socks5
            proxy ip: 10.0.1.101
            port: 1080
            username: voaleproxy
            passs: ...
            


#### Acrobat Reader

    Preferences:
        Accessibility:
            Always use Page Layout Style: Single Continous
            Always use Zoom Setting: Fit Page
        Documents:
            Remember current state of Tools Pane

#### Evernote

    Preferences - Application:
            Keep a copy of my notes on this device at sign-out: OFF

#### Telegram

    Preferences - General:
        Show Icon in Menu Bar: OFF

#### VLC

    Preferences - Interface:
        Display VLC status menu icon: OFF

#### Docker

    Preferences
        - General
            Send usage statistics : OFF
        - Experimental features
            Use the new Virt framework : On
            Enable VirtioFS accelerated sharing : On

## UNPAID

#### Multitouch:

    SystemPreferences - Security&Privacy - Privacy - Accessibility
        Multitouch : On

    Multitouch:
        Settings:
            Start on login : On
            Show menu bar icon : OFF
        Trackpad:
            - Two Finger:
                Rest one, tap one to the left:
                    Click: Middle Click
                Rest one, tap one to the right:
                    Click: Right Click
                Rest one, swipe down one to the left:
                    Apps with tabs: Switch tabs left
                Rest one, swipe up one to the left:
                    Apps with tabs: Switch tabs right
            - Four Finger:
                Click with four touches: -
                Tap with four touches:
                    macOS Keys & Shortcuts: Look up word under cursor (^ CMD D)
                    Focus window under cursor list: ON
                    Double tap: ON
                Swipe down with four:
                    Window Management: Minimize window under cursor

#### PopClip

    SystemPreferences - Security&Privacy - Privacy - Accessibility:
        PopClip: On

    Install extensions:
        - Mate Translate
        - Things3

    PopClip:
        Home:
            Start at login: ON
            Show in menu bar: OFF
        Actions:
            - Say
            - Copy(set show as icon)
            - Mate Translate
            - Things3

#### Contexts

    SystemPreferences - Security&Privacy - Privacy - Accessibility
        Contexts : On

    Contexts -
        Welcome - Launch Contexts at login
        Sidebar - Show sidebar on : No display
        Search - Search with : Hyper + Space - Fast Search with : Fn-characters : Off

## Only Rosetta

#### Winbox

    SystemPreferences - Security&Privacy - Firewall
        wineserver : Block incoming connections

## Check list

    lsof -Pn +c 35 | grep LISTEN                  # listen ports
    smartctl -x disk0                       # if data written 10Tb for 2weeks = it's bad
    iostat -w1 disk0                        # load average must <=2
    tmutil listbackups                      # view backup on Time Capsule(i.e RaspberryPi)
    tmutil listlocalsnapshots /             # view local snapshots
    tmutil deletelocalsnapshots /
