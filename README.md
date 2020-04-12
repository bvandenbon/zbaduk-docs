# ZBaduk documentation

This is the documentation of the website https://www.zbaduk.com which is dedicated to the board game Go/Baduk/WeiQi.

## Getting started

Visit the website, click Login.
Underneath the login button there is a registration link.
Or go directly to https://www.zbaduk.com/register

## Overview of tools

ZBaduk offers 4 tools.

1) Bot
2) Editor
3) Smart Review
4) Stored games

## Smart Review

### Purpose

The smart review tool uses LeeLa Zero to review your go game records.

### Connecting

After opening the Smart Review screen, a popup appears to connect to a server.
ZBaduk uses dedicated servers for GPU calculation.

![Connection screen](https://user-images.githubusercontent.com/20482760/58879024-f6019b80-86d4-11e9-9045-ae491acc6a8d.png)

You can just click the "Connect" button next to one of the servers.
After connecting, just click the "Start" button.

### Workspace

This is an overview that shows the names of the different parts of the layout. We will use these names throughout this manual.

![Workspace components](https://user-images.githubusercontent.com/20482760/58879352-c8692200-86d5-11e9-8532-34a1e9bcf146.png)

### Navigation

There are several ways, to navigate through game files.

1) You can use the navigation buttons underneath the board.
2) You can click the chart or the game tree

![Basic navigation](https://user-images.githubusercontent.com/20482760/58879683-7e347080-86d6-11e9-983f-b015dec80614.png)

### Add / Remove variations

To add variations, you can simply click the board.

![Add variations](https://user-images.githubusercontent.com/20482760/58880407-14b56180-86d8-11e9-8252-79162744cfa3.png)

To remove a variation, you select the start of the variation, and click the remove button in the general toolbar.

![Remove variation](https://user-images.githubusercontent.com/20482760/58880621-a1601f80-86d8-11e9-92cb-d826555b5529.png)

If you tried to remove a big branch, then a confirmation will be asked. This protects us against accidentally removing the wrong branch.

![Remove warning](https://user-images.githubusercontent.com/20482760/58881380-63fc9180-86da-11e9-9fe6-051b1cf96b3e.png)

### Use AI to analyze your games

To use AI, you should first be connected to an AI server. This is what the "connection dialog" was about at startup.
To verify quickly whether you are connected, check the color of the connect button.

![Connection status](https://user-images.githubusercontent.com/20482760/58880965-6d392e80-86d9-11e9-949b-fa7ac7016e66.png)

Once you are connected, 2 buttons become available:

![Connection modes](https://user-images.githubusercontent.com/20482760/58881074-b12c3380-86d9-11e9-9562-3c4ed81ee91a.png)

1) "Analyze this" : gathers statistics for the game record position that you are looking at. If you navigate through the game record, the computer analysis will follow you, and will always calculate for the visible position.

2) "Analyze full game" : gthers statistics for the entire game record, in the background. The goal of this mode is to gather enough data to create a smooth winrate chart. The winrate chart is useful for detecting big winrate swings, and thus can be used to quickly detect the losing/winning moves of the game record.

### Reading statistics

Statistics are shown as an overlay on the board.

![Winrates on the board](https://user-images.githubusercontent.com/20482760/79080740-d2a57500-7d17-11ea-926d-fd246c7facc3.jpg)

The move(s) with the highest decision value will be shown in blue. Other move candidates will be shown in colors ranging from green to red. The color is determined by their difference compared to the best move. 

Remark: Even if there is no chance left to win, the best moves will still be shown in green. The actual value does not influence the color, only the difference with the best move impacts the color.

### Winrate vs Decision

2 closely related statistics are the "winrate" and the "decision". The winrate estimates the chances for a player to win the game. However, the winrate does not take in account the number of playouts. Sometimes a move with a high winrate may have only a couple of playouts, and may not be very reliable. The decision value by contrast goes one step further than a simple winrate and takes this risk in account.

By default, the winrate and decision value are shown from the perspective of the active player, and will switch sides with each play. _(e.g. If black has a winrate of 40%, but it's white's turn, then it will show 60%.)_ However, this can be configured to be shown fixed from Black or White's perspective as well. Refer to the "UI Settings" screen for this:

![image](https://user-images.githubusercontent.com/20482760/79080954-590e8680-7d19-11ea-8a10-129a0d1ef3c3.png)


### Zoom

ZBaduk tries to adjust its user interface to get the most out of your system. It will re-arrange items to make the board itself as big as possible. 

Having said that, on smart phones it can be clumsy to click the correct intersection. For this reason, the board will automatically zoom when you click it. This behavior is designed to be only active on mobile devices.

![Auto-Zoom](https://user-images.githubusercontent.com/20482760/59000749-23049a00-880c-11e9-9382-2bfe17d634e2.png)

### Coordinates

In the "More..." > "UI Settings" menu you can configure how the coordinates should be oriented, or you can hide them as well.

![image](https://user-images.githubusercontent.com/20482760/79081115-accd9f80-7d1a-11ea-96ac-b04d86441e5d.png)

