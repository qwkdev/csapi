# CURRENTLY OUT OF DATE, AS I HAVENT ADDED ANY SKINS FROM THE ARMORY UPDATE ONWARDS
# WILL UPDATE SOON (eventually)

# JSON LINKS: [V2](https://raw.githubusercontent.com/qwkdev/csapi/main/data2.json), [V1](https://raw.githubusercontent.com/qwkdev/csapi/main/data.json)

# V2 or V1?

**If you have used other apis for cs skins, V2 is what you will be used to.**

### V2 HAS AN ELEMENT FOR EACH SKIN'S POSSIBLE EXTERIOR AND TYPE

V2 is useful for projects like games, that need a separate item for each exterior and type (such as "AWP | Dragon Lore (Factory New)", "StatTrak™ AWP | Dragon Lore (Factory New)", "AWP | Dragon Lore (Minimal Wear)", etc...)



### V1 JUST HAS AN ELEMENT FOR EACH SKIN

V1 is useful for projects that just need data for a skin (eg: float caps, gen code, etc...) although you can still get all the data for each element in V1, in V2. (You aren't missing out on anything by using V2)



# CSAPI

# V2

### Layout

The JSON is layed out like this: (example for an **Souvenir AWP | Dragon Lore (Factory New)**)



**full name of item** ("Souvenir AWP | Dragon Lore (Factory New)"): {

        "type": **type of item** ("Souvenir"),

        "exterior": **exterior of item** ("Factory New"), [^1]

        "image": **link to image of item** ("https://steam..."), [^2]

        "inspect": {

                "gen": **gen code of item** ("!gen 9 344"),

                "link": **in-game inspect link** ("steam://rungame/...") [^3]

        },

        "phase": **phase** ("Emerald"), **!!! ONLY EXISTS FOR DOPPLERS !!!**

        "full-name": **name of item** ("Souvenir AWP | Dragon Lore (Factory New)"),

        "name": **name of skin** ("AWP | Dragon Lore"),

        "weapon": **weapon name** ("AWP"),

        "weapon-catalog": **in-game ID of weapon** (9),

        "csgostash-id": **the id on csgostash.com/skin/[ID]** (422),

        "finish": **the skin** ("Dragon Lore"),

        "is-doppler": **if the skin is a doppler/gamma doppler** (false),

        "finish-catalog": **in-game ID of finish** (344),

        "finish-style": **style of finish** ("Custom Paint Job"), [^4]

        "rarity": **rarity of skin** ("Covert"),

        "color": **color of rarity** ("#eb4b4b"),

        "float-caps": **list of float caps [min, max]** ([0, 0.7]), [^4]

        "possible": **list of each possible item** (["Factory New", "Minimal Wear", ..., "Souvenir Factory New", ...]), [^1]

        "types": **list of each possible type of item** (["Normal", "Souvenir"]),

        "date-added": {

                "text": **date added text** ("1 July 2014"),

                "date": **date added** ("1/7/2014"),

                "unix": **date added in unix** (1404172800)

        }

}

**FULL EXAMPLE**

```json
"Souvenir AWP | Dragon Lore (Factory New)": {
  "type": "Souvenir",
  "exterior": "Factory New",
  "image": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu5Mx2gv2PrdSijAWwqkVtN272JIGdJw46YVrYqVO3xLy-gJC9u5vByCBh6ygi7WGdwUKTYdRD8A/512fx384f",
  "inspect": {
    "gen": "!gen 9 344",
    "link": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198299749713A7013114583D3180113772518061157"
  },
  "full-name": "Souvenir AWP | Dragon Lore (Factory New)",
  "name": "AWP | Dragon Lore",
  "weapon": "AWP",
  "weapon-catalog": 9,
  "csgostash-id": 422,
  "finish": "Dragon Lore",
  "is-doppler": false,
  "finish-catalog": 344,
  "finish-style": "Custom Paint Job",
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": [
    0,
    0.7
  ],
  "possible": [
    "Factory New",
    "Minimal Wear",
    "Field-Tested",
    "Well-Worn",
    "Battle-Scarred",
    "Souvenir Factory New",
    "Souvenir Minimal Wear",
    "Souvenir Field-Tested",
    "Souvenir Well-Worn",
    "Souvenir Battle-Scarred"
  ],
  "types": [
    "Normal",
    "Souvenir"
  ],
  "date-added": {
    "text": "1 July 2014",
    "date": "1/7/2014",
    "unix": 1404172800
  }
}
```

# MORE EXAMPLES

### GAMMA DOPPLER

```json
"★ StatTrak™ Karambit | Gamma Doppler Emerald (Factory New)": {
  "type": "StatTrak™",
  "exterior": "Factory New",
  "image": "https://csgostash.com/storage/img/skin_variants/s782_emerald.png?id=413d1a4e2a1bd899954ecb26eea10096",
  "inspect": {
    "gen": "!gen 507 568",
    "link": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198001812949A6599931946D14334573342458081943"
  },
  "phase": "Emerald",
  "full-name": "★ StatTrak™ Karambit | Gamma Doppler Emerald (Factory New)",
  "name": "★ Karambit | Gamma Doppler",
  "weapon": "Karambit",
  "weapon-catalog": 507,
  "csgostash-id": 782,
  "finish": "Gamma Doppler",
  "is-doppler": true,
  "finish-catalog": 568,
  "finish-style": "Anodized Multicolored",
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": [
    0,
    0.08
  ],
  "possible": [
    "StatTrak™ Factory New",
    "StatTrak™ Minimal Wear",
    "Factory New",
    "Minimal Wear"
  ],
  "types": [
    "Normal",
    "StatTrak™"
  ],
  "date-added": {
    "text": "16 June 2016",
    "date": "16/6/2016",
    "unix": 1466035200
  }
}
```

### VANILLA

```json
"★ Butterfly Knife | Vanilla (Factory New)": {
  "type": "Normal",
  "exterior": "Factory New",
  "image": "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/weapons/base_weapons/weapon_knife_butterfly.794147e84a4e9426202d45145910cbb007797ce5.png",
  "inspect": {
    "gen": "!gen 515",
    "link": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20M633137629095046309A6485249749D328415975175144145"
  },
  "full-name": "★ Butterfly Knife | Vanilla (Factory New)",
  "name": "★ Butterfly Knife | Vanilla",
  "weapon": "Butterfly Knife",
  "weapon-catalog": 515,
  "csgostash-id": 452,
  "finish": "Vanilla",
  "is-doppler": false,
  "finish-catalog": 0,
  "finish-style": null,
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": null,
  "possible": [
    "Factory New",
    "StatTrak™ Factory New"
  ],
  "types": [
    "Normal",
    "StatTrak™"
  ],
  "date-added": {
    "text": "1 July 2014",
    "date": "1/7/2014",
    "unix": 1404172800
  }
}
```



# V1

### Layout

The JSON is layed out like this: (example for an **AWP | Dragon Lore**)



**name of skin** ("AWP | Dragon Lore"): {

        "name": **name of skin** ("AWP | Dragon Lore"),

        "weapon": **weapon name** ("AWP"),

        "weapon-catalog": **in-game ID of weapon** (9),

        "csgostash-id": **the id on csgostash.com/skin/[ID]** (422),

        "finish": **the skin** ("Dragon Lore"),

        "is-doppler": **if the skin is a doppler/gamma doppler** (false), [^5]

        "finish-catalog": **in-game ID of finish** (344), [^6]

        "finish-style": **style of finish** ("Custom Paint Job"), [^4]

        "rarity": **rarity of skin** ("Covert"),

        "color": **color of rarity** ("#eb4b4b"),

        "float-caps": **list of float caps [min, max]** ([0, 0.7]), [^4]

        "images": **JSON of each wear and it's image** ({"Factory New": "https://steam...", "Minimal Wear": "https://steam...", etc...}), [^7] [^1]

        "possible": **list of each possible item** (["Factory New", "Minimal Wear", ..., "Souvenir Factory New", ...]), [^1]

        "types": **list of each possible type of item** (["Normal", "Souvenir"]),

        "inspect": {

                "gen": **gen code** ("!gen 9 344"), [^8]

                "links": **each wears in-game link** ({"Factory New": "steam://rungame...", "Minimal Wear": "steam://rungame...", etc...}) [^3] [^9]

        },

        "date-added": {

                "text": **date added text** ("1 July 2014"),

                "date": **date added** ("1/7/2014"),

                "unix": **date added in unix** (1404172800)

        }

}

**FULL EXAMPLE**

```json
"AWP | Dragon Lore": {
  "name": "AWP | Dragon Lore",
  "weapon": "AWP",
  "weapon-catalog": 9,
  "csgostash-id": 422,
  "finish": "Dragon Lore",
  "is-doppler": false,
  "finish-catalog": 344,
  "finish-style": "Custom Paint Job",
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": [
    0,
    0.7
  ],
  "images": {
    "Factory New": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu5Mx2gv2PrdSijAWwqkVtN272JIGdJw46YVrYqVO3xLy-gJC9u5vByCBh6ygi7WGdwUKTYdRD8A/512fx384f",
    "Minimal Wear": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu5Mx2gv2PrdSijAWwqkVtN272JIGdJw46YVrYqVO3xLy-gJC9u5vByCBh6ygi7WGdwUKTYdRD8A/512fx384f",
    "Field-Tested": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu5cB1g_zMu9Wk2ATh_0tkMWrzLY7BIQM2NArQq1O9kL_qgJTt6Ziam3Bh6SR3sHfD30vgriIWFx4/512fx384f",
    "Well-Worn": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu5cB1g_zMu9Wk2ATh_0tkMWrzLY7BIQM2NArQq1O9kL_qgJTt6Ziam3Bh6SR3sHfD30vgriIWFx4/512fx384f",
    "Battle-Scarred": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpot621FAR17P7NdTRH-t26q4SZlvD7PYTQgXtu4MBwnPCPoYqtjFHsqEE5Zj-gddDGegZsMwnVrwW8wbzv0cXptMyayXZnvHJ0tGGdwUIocz3_kQ/512fx384f"
  },
  "possible": [
    "Factory New",
    "Minimal Wear",
    "Field-Tested",
    "Well-Worn",
    "Battle-Scarred",
    "Souvenir Factory New",
    "Souvenir Minimal Wear",
    "Souvenir Field-Tested",
    "Souvenir Well-Worn",
    "Souvenir Battle-Scarred"
  ],
  "types": [
    "Normal",
    "Souvenir"
  ],
  "inspect": {
    "gen": "!gen 9 344",
    "links": {
      "Factory New": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198299749713A7013114583D3180113772518061157",
      "Minimal Wear": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198254145867A7013781737D3026562455898750633",
      "Field-Tested": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198254162479A6987335927D346401843859193579",
      "Well-Worn": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198251568662A7013590656D10098769016625060393",
      "Battle-Scarred": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198253336261A6934848330D12289449051849505839"
    }
  },
  "date-added": {
    "text": "1 July 2014",
    "date": "1/7/2014",
    "unix": 1404172800
  }
}
```



# MORE EXAMPLES:

### GAMMA DOPPLER

```json
 "★ Karambit | Gamma Doppler": {
  "name": "★ Karambit | Gamma Doppler",
  "weapon": "Karambit",
  "weapon-catalog": 507,
  "csgostash-id": 782,
  "finish": "Gamma Doppler",
  "is-doppler": true,
  "finish-catalog": {
    "Phase 1": 569,
    "Phase 2": 570,
    "Phase 3": 571,
    "Phase 4": 572,
    "Emerald": 568
  },
  "finish-style": "Anodized Multicolored",
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": [
    0,
    0.08
  ],
  "images": {
    "Phase 1": "https://csgostash.com/storage/img/skin_variants/s782_phase1.png?id=40a8ac36051bedd881fda234f9afe9ba",
    "Phase 2": "https://csgostash.com/storage/img/skin_variants/s782_phase2.png?id=3e27528bcd6721c50647b83edc1cab44",
    "Phase 3": "https://csgostash.com/storage/img/skin_variants/s782_phase3.png?id=7c36d22a6f119f27b845365a967b2afb",
    "Phase 4": "https://csgostash.com/storage/img/skin_variants/s782_phase4.png?id=4d9633cb3d5ac7927bf1c2f4c63d46d3",
    "Emerald": "https://csgostash.com/storage/img/skin_variants/s782_emerald.png?id=413d1a4e2a1bd899954ecb26eea10096"
  },
  "possible": [
    "StatTrak™ Factory New",
    "StatTrak™ Minimal Wear",
    "Factory New",
    "Minimal Wear"
  ],
  "types": [
    "Normal",
    "StatTrak™"
  ],
  "inspect": {
    "gen": {
      "Phase 1": "!gen 507 569",
      "Phase 2": "!gen 507 570",
      "Phase 3": "!gen 507 571",
      "Phase 4": "!gen 507 572",
      "Emerald": "!gen 507 568"
    },
    "links": {
      "Phase 1": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198120045401A6643376124D9685096593643756275",
      "Phase 2": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561197981264868A6626619635D2894165744253391101",
      "Phase 3": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198148995613A6614952442D7971969508545099517",
      "Phase 4": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198013327613A6608802478D2742248576393351871",
      "Emerald": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198001812949A6599931946D14334573342458081943"
    }
  },
  "date-added": {
    "text": "16 June 2016",
    "date": "16/6/2016",
    "unix": 1466035200
  }
}
```

### VANILLA

```json
"★ Butterfly Knife | Vanilla": {
  "name": "★ Butterfly Knife | Vanilla",
  "weapon": "Butterfly Knife",
  "weapon-catalog": 515,
  "csgostash-id": 452,
  "finish": "Vanilla",
  "is-doppler": false,
  "finish-catalog": 0,
  "finish-style": null,
  "rarity": "Covert",
  "color": "#eb4b4b",
  "float-caps": null,
  "images": {
    "Factory New": "https://steamcdn-a.akamaihd.net/apps/730/icons/econ/weapons/base_weapons/weapon_knife_butterfly.794147e84a4e9426202d45145910cbb007797ce5.png"
  },
  "possible": [
    "Factory New",
    "StatTrak™ Factory New"
  ],
  "types": [
    "Normal",
    "StatTrak™"
  ],
  "inspect": {
    "gen": "!gen 515",
    "links": {
      "Factory New": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20M633137629095046309A6485249749D328415975175144145"
    }
  },
  "date-added": {
    "text": "1 July 2014",
    "date": "1/7/2014",
    "unix": 1404172800
  }
}
```



[^1]: vanilla knifes are classed as "Factory New"

[^2]: image is hosted on csgostash for dopplers

[^3]: a link may be null for some edge cases
eg: {"Factory New": null, "Minimal Wear": "steam://rungame/...", etc.}

[^4]: becomes null for vanilla knifes

[^5]: this is useful because "finish-catalog" becomes a list of the finish catalogs for each phase rather than being just an integer

[^6]: changes to include phases (and gems) for dopplers
eg: {"Phase 1": 569, "Phase 2": 570, etc.}

[^7]: becomes images of each phase (and gem) for dopplers, rather than exterior
eg: {"Phase 1": "https://...", "Phase 2": "https://...", etc.}

[^8]: changes to include phases (and gems) for dopplers
eg: {"Phase 1": "!gen ...", "Phase 2": "!gen ...", etc.}

[^9]: becomes links of each phase (and gem) for dopplers, rather than exterior
eg: {"Phase 1": "steam://rungame...", "Phase 2": "steam://rungame...", etc.}
