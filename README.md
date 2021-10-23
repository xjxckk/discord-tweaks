# BetterDiscord Custom CSS Tweaks
Includes inline channel tabs and hiding of channel tabs when in settings

![BetterDiscord Custom CSS Tweaks](https://github.com/xjxckk/discord-tweaks/blob/main/preview.png)

### How to setup:
* Install [BetterDiscord](https://betterdiscord.app)
* Install [Zelk](https://betterdiscord.app/theme/zelk/)
* Install [ChannelTabs](https://betterdiscord.app/plugin/ChannelTabs/)
* Copy the Custom CSS below and save it in the Custom CSS section in Discord settings


```
/* Channel tabs inline */
/* Move main container up */
.layers-3iHuyZ.layers-3q14ss {margin-top: -50px}

/* Move main section (that isn't the server list siderbar) down */
.base-3dtUhz {margin-top: 45px}

/* Container div (includes settings menu button */
#channelTabs-container {margin-left: 62px}

/* Actual tab container div */
.channelTabs-tabContainer {
    min-height: calc(var(--channelTabs-tabHeight) + 10px) !important;
    background-color: var(--background-tertiary) !important
}

/* Resize tab */
.channelTabs-tab {
    margin-top: 4px !important;
    height: calc(var(--channelTabs-tabHeight) - 12px) !important;
    font-size: calc(var(--channelTabs-tabTextSize) - 2px) !important;
    background-color: var(--background-tertiary) !important
}

/* Colour of selected tab */
.channelTabs-tab.channelTabs-selected {background: var(--background-secondary) !important}

/* Colour of close tab button */
.channelTabs-closeTab {background: var(--interactive-muted) !important}

/* Hide tab favicons */
.channelTabs-tabIcon {display: none !important}

/* Format tab title text */
.channelTabs-tabName {
    margin-left: 10px !important; /* Account for hiding of icon */
    line-height: 20px; /* Vertically center text */
}

/* Show settings page above tabs - settings is an overlay so cant switch between tabs while it is open */
.standardSidebarView-3F1I7i {z-index: 1001}

/* End channel tabs inline */

/* Hide Nitro tab */
#private-channels [href="/store"] {display: none}
/* Hide Nitro gift button */
.buttons-3JBrkn > button {display: none}
/* Hide Gif button */
.buttons-3JBrkn > div:nth-child(3) {display: none}
/* Hide stickers button */
.stickerButton-3OEgwj {display: none}
```
