# Aliano Roleplay Train System for FiveM

![Bannière du script aliano_train_system](https://i.ibb.co/FqzdLWf1/aliano-train-system-fivem-readme.png)

## Description

A realistic train transportation script for FiveM servers featuring interactive stations, ticket purchasing, and immersive travel sequences.

## Features

- **12+ Detailed Stations** across Los Santos and Blaine County
- **Interactive Ticket Booths** with marker-based UI
- **Dynamic Departure System** with real-time countdowns
- **Immersive Travel Experience** with video sequences
- **OX Inventory Integration** for ticket payments
- **Clean Money/Black Money** payment options
- **Realistic Station Information** (platforms, delays, travel times)
- **Responsive NUI Interface** with station images

## Installation

1. Add `aliano_train` to your resources folder
2. Add `ensure aliano_train` to your server.cfg
3. Configure stations in `config.lua`
4. Add your station images to `web/images/`
5. Add travel videos to `web/videos/`

## Configuration

`config.lua` to customize:

```lua
Config = {
    Stations = {
        {
            name = "LS Airport",
            label = XX,
            coords = XX,
            ticketBooth = XX,
            image = XX,
            time = XX,
            platform = XX,
            status = XX,
        },
        -- More stations...
    },
    TicketPrice = 100, -- Default ticket price, you can edit the HTML also
    Messages = {
        xxx : xxx,
        xxx : xxx,
        xxx : xxx,
    }
}
```

## Dependencies

- [ox_inventory](https://github.com/overextended/ox_inventory) (or edit server.lua for other ESX/QB systems)
- FiveM NUI compatible resource

## To change the video

1. Place MP4 videos in `./videos/`
2. Name it `travel_1.mp4` and remove mine.
3. Reference in client.lua: `videoFile = "travel_1.mp4"` & trainGui.js : `data.videoFile || "travel_1.mp4"`

## Image Requirements

- Station images should be WebP format (recommended 492\*300~)
- Place in `client/images/`
- Match filenames to config (e.g., "lsia.webp")

## Troubleshooting

- **NUI errors**: Ensure all web files load properly
- **Payment issues**: Verify ox_inventory is properly installed
- **Marker problems**: Check coordinates in config
- **Video issues**: Ensure MP4s are properly encoded (H.264)

## License

This resource is provided as-is. Modification and redistribution permitted with attribution.

---

**Created by Aliano**  
_Need help? Contact me on [Discord](https://discord.gg/Jcuramxw)

## Purchase

Available for purchase on my Tebex store:  
[Download on Tebex](https://shorturl.at/lrZN8)

## Preview (click on the image)

[![Présentation YouTube du script](https://img.youtube.com/vi/e2N21F6oYAs/maxresdefault.jpg)](https://www.youtube.com/watch?v=e2N21F6oYAs)

---

_See you soon! Aliano._
