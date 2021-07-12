<!-- Badge for License -->
<div align="right">

  [![](https://img.shields.io/github/license/MUD-TW/RanvierMUD-Chaos.svg?style=flat-square)](./LICENSE)

</div>

<!-- Logo and Title -->
<div align="center">
  <img src="https://i.imgur.com/yoU8Rbc.png" alt="Chaos" height="150px">

# 洪荒世界（The Chaos）

🌌 _An example MUD world based on [RanvierMUD](https://github.com/RanvierMUD/ranviermud) MUD game engine._<br/>
_基於 [RanvierMUD](https://github.com/RanvierMUD/ranviermud) 遊戲引擎架站的範例遊戲世界_

</div>

## 快速啟動

```bash
# 下載專案
$ git clone https://github.com/MUD-TW/RanvierMUD-Chaos.git

# 安裝依賴
$ cd RanvierMUD-Chaos
$ npm install && npm run init

# 啟動服務
$ npm run start
```

## 登入流程

```
                      intro (MOTD)
                        |
      (new account) __login__  (existing account)
                   /         \
     create-account           password----------------------
        |                            |                     |
  change-password              choose-character      change-password
        |                            |
  create-player                      |
        |                            |
  player-name-check                  |
        |                            |
  finish-player                      |
        |__________________________done (add player to game world)
                                     |
                                   commands
             (command prompt, all player input after login goes through this event)
```

## 授權許可

Licensed under the MIT License, Copyright © 2021-present MUD-TW (Multi-User Dungeon Taiwan).
