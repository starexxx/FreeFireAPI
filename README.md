# API Documentation
<b>Last Update</b>: 20 January 2025<br>
Join our channel for latest API Key!!
<a href="https://t.me/starexxxxxx">Join Now!</a>
# Account Information
<b>Endpoint</b>: `/profile`<br>
<b>Method</b>: `GET`<br>
<b>Description</b>:
This endpoint retrieves account information based on the specified region and user ID.

### Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| uid     | integer | Yes      | The user ID.
| region  | string | Yes      | The region code (IND, BR, SG, RU, ID, TW, US, VN, TH, ME, PK, CIS, BD).
| key     | string | Yes      | API Key.|
### Request Example
```http
GET https://freefireinfo.vercel.app/profile?region={region}&uid={player_uid}&key={Api_Key}
```
### Response Example
```json
{
  "status": "success",
  "rule": "Shah G Creator",
  "Region": "SG",
  "PlayerUID": "12345678",
  "data": {
    "ProfileInfo": {
      "AvatarID": 902000154,
      "BPBadges": 79,
      "BPID": 1001000080,
      "BannerID": 901045005,
      "CreateTime": 1512595169,
      "EXP": 1970046,
      "LastSeen": 1737277460,
      "Level": 66,
      "Likes": 3404621,
      "Nickname": "FB:ㅤ@GMRemyX",
      "Region": "SG",
      "BrSeason": 43,
      "ProfileType": 1,
      "BrMaxRank": 214,
      "BrRankPoint": 2489,
      "CsMaxRank": 220,
      "CsRankPoint": 120,
      "EquipGun": [907103421, 912041002, 914047001],
      "LoginVersion": "OB47",
      "Role": 4,
      "ShowBrRank": true,
      "ShowCsRank": true,
      "Title": 904090023
    },
    "CollectionInfo": {
      "EquipOutfit": [203047032, 204000884, 211046056, 214039014, 205046033],
      "EquipSkills": [16, 706, 8, 1, 16, 3806, 8, 2, 16, 2506, 8, 3, 16, 1706]
    },
    "GuildInfo": {
      "GuildCapacity": 55,
      "GuildID": "60893361",
      "GuildLevel": 7,
      "GuildMember": 50,
      "GuildName": "MᴜᴍᴍʏEᴠᴀTᴇᴀᴍ",
      "GuildOwner": "12345678"
    },
    "captainBasicInfo": {
      "EquipGun": [907103421, 912041002, 914047001],
      "accountId": "12345678",
      "accountType": 1,
      "badgeCnt": 79,
      "badgeId": "1001000080",
      "bannerId": "901045005",
      "createAt": "1512595169",
      "csMaxRank": 220,
      "csRank": 220,
      "csRankingPoints": 120,
      "Exp": 1970046,
      "headPic": "902000154",
      "lastLoginAt": "1737277460",
      "PetLevel": 66,
      "liked": 3404621,
      "maxRank": 214,
      "nickname": "FB:ㅤ@GMRemyX",
      "rank": 214,
      "rankingPoints": 2489,
      "region": "SG",
      "releaseVersion": "OB47",
      "seasonId": 43,
      "showBrRank": true,
      "showCsRank": true,
      "title": 904090023
    },
    "HonorScoreInfo": {
      "HonorScore": 100,
      "EndTime": "1737511382",
      "StartTime": "1737252182",
      "rewardState": 1
    },
    "PetInfo": {
      "Exp": 6000,
      "PetID": 1300000071,
      "isEquip": true,
      "PetLevel": 7,
      "name": "SiNo",
      "PetSkill": 1315000009,
      "PetSkin": 1310000071
    },
    "ProfilePage": {
      "Language": "Language_English",
      "PreferMode": "Prefermode_BR",
      "ProfileBio": "FB & YT GM Remy | TikTok :gmremyx | IG GM Remy"
    }
  }
}
```
# Craftland Map Info

<b>Endpoint</b>: `/map`  <br>
<b>Method</b>: `GET` <br>
<b>Description</b>: The Craftland Map Info API provides details about custom maps in Free Fire, including title, description, creator, size, game mode, realtime likes and subscriptions.

### Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| code     | string | Yes      | Map Code.
| region  | string | Yes      | The region code (IND, BR, SG, RU, ID, TW, US, VN, TH, ME, PK, CIS, BD).
| key     | string | Yes      | Api Key.|
### Request Example
```http
GET https://freefireinfo.vercel.app/map?region={region}&code={map_code}&key={Api_Key}
```
### Response Example
```json
{
  "status": "success",
  "data": {
    "rule": "Shah G Creator",
    "region": "IND",
    "lang": "en",
    "Craftland Map Details": {
      "MapCode": "#FREEFIRE6CCBEEB07F9728C99868FA34BC3B8C2A7490",
      "Creator": "Joy5b0x7H6o",
      "Title": "Bermuda: Preying Party",
      "ShortCode": "FFBBPP",
      "Description": "1. Upgrade and equip Chips in the Safe House to prepare for the fight.\n2. Excess supplies can be stored in Vault or sold for Coins.\n3. Enter the battleground and eliminate enemies to loot their supplies, then take the supplies to the Evacuation Point!",
      "Subscribers": 91573,
      "Likes": 7093,
      "Teams": 30,
      "PlayAverage": 392,
      "Rounds": 1,
      "Mode": "Customize"
    }
  }
}
```
# Free Fire Events

<b>Endpoint</b>: `/event`<br>
<b>Method</b>: `GET`<br>
<b>Description</b>: The Free Fire Incoming Event API provides real-time details about upcoming in-game events, including event names, start and end dates, rewards, and banners.

### Query Parameters

| Parameter | Type   | Required | Description                   |
|-----------|--------|----------|-------------------------------|
| region  | string | Yes      | The region code (IND, BR, SG, RU, ID, TW, US, VN, TH, ME, PK, CIS, BD).
| Valid Regions (ID, IND, NA, PK, BR, ME, SG, BD, TW, TH, VN, CIS, EU,SAC)
| key     | string | Yes      | Api Key |
### Request Example
```http
GET https://freefireinfo.vercel.app/event?region={region}&key={Api_Key}
```
### Response Example
```json
{
  "status": "success",
  "rule": "Shah G Creator",
  "region": "IND",
  "Events Info": [
    {
      "Title": "Ninja Training: Stamina",
      "Description": "",
      "Start": "1737412200",
      "End": "1737498599",
      "Banner": "https://dl-tata.freefireind.in/common/Local/IND/config/1750x1080_NinjaTrainingStaminaSplashIND_en.jpg",
      "Redirect": ""
    },
    {
      "Title": "Naruto Main CG",
      "Description": "",
      "Start": "1737325800",
      "End": "1737412199",
      "Banner": "https://dl-tata.freefireind.in/common/Local/IND/config/1750x1070_NarutoMainCGSplashIND_en.jpg",
      "Redirect": ""
    },
    {
      "Title": "Naruto Royale: NINE TAILS SKYWING x NARUTO M4A1",
      "Description": "",
      "Start": "1737325800",
      "End": "1737412199",
      "Banner": "https://dl-tata.freefireind.in/common/Local/IND/config/1750x1070_NarutoRoyaleSPlashIND_en.jpg",
      "Redirect": ""
    },
    {
      "Title": "Free Ninja Emote Trials (Login Mission)",
      "Description": "",
      "Start": "1737239400",
      "End": "1737325799",
      "Banner": "https://dl-tata.freefireind.in/common/Local/IND/config/1750x1080_FreeNinjaEmoteTrialsSplashIND_en.jpg",
      "Redirect": ""
    },
    {
      "Title": "LESS IS MORE",
      "Description": "",
      "Start": "1737239400",
      "End": "1737325799",
      "Banner": "https://dl-tata.freefireind.in/common/Local/IND/config/1750x1070_LessIsMoreSplashIND_en.jpg",
      "Redirect": ""```
    }
  ]
}
