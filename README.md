# LINK TO JSON: [HERE](https://raw.githubusercontent.com/qqwkk/csapi/main/data.json)



# CSAPI



### Layout

The JSON is layed out like this: (example for an **AWP | Dragon Lore**)



**name of skin** ("AWP | Dragon Lore"): {

        "name": **name of skin** ("AWP | Dragon Lore"),

        "weapon": **weapon name** ("AWP"),

        "weapon-catalog": **in-game ID of weapon** (9),

        "csgostash-id": **the id on csgostash.com/skin/[ID]** (422),

        "finish": **the skin** ("Dragon Lore"),

        "is-doppler": **if the skin is a doppler/gamma doppler** ("False"), [^1]

        "finish-catalog": **in-game ID of finish** (344), [^2]

        "finish-style": **style of finish** ("Custom Paint Job"), [^3]

        "rarity": **rarity of skin** ("Covert"),

        "color": **color of rarity** ("#eb4b4b"),

        "float-caps": **list of float caps [min, max]** ([0, 0.7]), [^3]

        "images": **JSON of each wear and it's image** ({"Factory New": "https://steam...", "Minimal Wear": "https://steam...", etc...}),

        "possible": **list of each possible item** ("Factory New", "Minimal Wear", ..., "Souvenir Factory New", ...),

        "types": **list of each possible type of item** ("Normal", "Souvenir"),

        "inspect": {

                "gen": **gen code** ("!gen 9 344"),

                "links": **list of each wears in-game link** ({"Factory New": "steam://rungame...", "Minimal Wear": "steam://rungame...", etc...})

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
    "csgostash-id": "422",
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
    "csgostash-id": "782",
    "finish": "Gamma Doppler",
    "is-doppler": true,
    "finish-catalog": [
        [
            569,
            "Phase 1"
        ],
        [
            570,
            "Phase 2"
        ],
        [
            571,
            "Phase 3"
        ],
        [
            572,
            "Phase 4"
        ],
        [
            568,
            "Emerald"
        ]
    ],
    "finish-style": "Anodized Multicolored",
    "rarity": "Covert",
    "color": "#eb4b4b",
    "float-caps": [
        0,
        0.08
    ],
    "images": {
        "Factory New": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpovbSsLQJf2PLacDBA5ciJlY20kPb5PrrukmRB-Ml0mNbR_Y3mjQCLpxo7Oy3tJIPBIVM4Zw7U81C7x7_q1sS8tM-bmntjs3Qq5S2MnBa3hxxLZuFn1-veFwu1gXfnHg/512fx384f",
        "Minimal Wear": "https://steamcommunity-a.akamaihd.net/economy/image/-9a81dlWLwJ2UUGcVs_nsVtzdOEdtWwKGZZLQHTxDZ7I56KU0Zwwo4NUX4oFJZEHLbXH5ApeO4YmlhxYQknCRvCo04DEVlxkKgpovbSsLQJf2PLacDBA5ciJlY20kPb5PrrukmRB-Ml0mNbR_Y3mjQWLpxo7Oy3tcIeUJABrMw7Xq1O_xOjmgsW4tZ-fzSRmuCVzsXrazhy1hR8aOrFpg-veFwszX91FHg/512fx384f"
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
        "gen": [
            [
                "!gen 507 569",
                "Phase 1"
            ],
            [
                "!gen 507 570",
                "Phase 2"
            ],
            [
                "!gen 507 571",
                "Phase 3"
            ],
            [
                "!gen 507 572",
                "Phase 4"
            ],
            [
                "!gen 507 568",
                "Emerald"
            ]
        ],
        "links": {
            "Factory New": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198254492039A7007319284D172861540519622905",
            "Minimal Wear": "steam://rungame/730/76561202255233023/+csgo_econ_action_preview%20S76561198299727584A7015466984D3341748720859469939"
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
    "csgostash-id": "452",
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
        "StatTrak™ Vanilla",
        "Vanilla"
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

---

[^1]: this is useful because "finish-catalog" becomes a list of the finish catalogs for each phase rather than being just an integer

[^2]: becomes a list of the finish catalogs for each phase rather than being just an integer
eg: [[418, "Phase 1"], [419, "Phase 2"], [420, "Phase 3"], [421, "Phase 4"], [415, "Ruby"], [416, "Sapphire"], [417, "Black Pearl"]]

[^3]: becomes null for vanilla knifes
