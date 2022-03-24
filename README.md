# LickHunterPro-Assistant
Assistant Software to manage LickHunterPro Bot using python and liquidation data from https://liquidation.atsutane.net

> ***Trading futures is very high risk and involves a risk of loss. Please consider carefully if such trading is appropriate for you. Past performance is not indicative of future results. Software and data on this page are for research purposes only and do not constitute investment recommendations or advice. Do your own research!***

![LHPA-UI](https://user-images.githubusercontent.com/6040550/121283129-33751100-c90d-11eb-8435-93f81acf2bfd.PNG)
![LHA-Webhook](https://user-images.githubusercontent.com/6040550/121284778-f6f6e480-c90f-11eb-965c-1c0d0cab4177.PNG)
![LHA-Menu](https://user-images.githubusercontent.com/6040550/121283197-4f78b280-c90d-11eb-8483-cc99fd1ac573.PNG)

## LickHunterPro-Assistant Features
- [x] Automatically choose pairs for trading base from balance, leverage and percentBal
- [x] Automatically choose lick value, long offset & short offset base on data from https://liquidation.atsutane.net
- [x] Discord Webhook support for notification and status change
- [x] Automatically transfer balance from future to spot.
- [x] Support using secondary take profit value when reach isolation mode.
- [x] Support emergency exit plan by reducing secondary take profit value into half when margin is over 50%
- [x] Interactive hotkey menu
- [x] Colorfull discord embed :D
- [ ] still building the list

## LickHunterPro-Assistant Known Issues
- [x] The script randomly freeze. Main loop broken. Need to close and it will work again.
- [x] Auto PercentBal not really working on Bybit Exchange
- [ ] still building the list

## LickHunterPro-Assistant Setup
Download the latest version from *https://github.com/AtsutaneDotNet/LickHunterPro-Assistant/releases*. Extract and put it inside LHP folders

![LHA setup](https://user-images.githubusercontent.com/6040550/134997297-3d252a2c-0874-4c9b-a9b6-b1d448b11e7f.PNG)

Just change *control.json* suitable to your need and run *LickHunterAssistant.exe*
```json
{
    "tradingSettings": {
        "maxPairs": "300",
        "maxPositions": "2",
        "IsoPercentage": "10",
        "PrimaryProfit": "0.8",
        "SecondaryProfit": "0.6",
        "EmergencyExit": "true",
        "EmergencyTrigger": "20",
        "EmergencyProfit": "0.4",
        "OverrideLongOffset": "0",
        "OverrideShortOffset": "0",
        "24hprice_limit": "21",
        "funding_limit": "0.1",
        "AutoIsolatedAndLevChange": "true",
        "margin_type": "ISOLATED"
    },
    "tradingPairs": {
        "whitelist": "",
        "CurrentPairs": "",
        "LastUsedPairs": "",
        "blacklist": ""
    },
    "tradingAI": {
        "autoPbal": "true",
        "autoMaxPos": "true",
        "LickValueType": "safe",
        "nominalValue": "6",
        "MaxMin": "false",
        "maxVwap": "12",
        "minVwap": "8"
    },
    "autoTransfer": {
        "status": "true",
        "limit": "10000",
        "increase_limit": "true",
        "percentage": "1"
    },
    "misc": {
        "bot_name": "Assistant",
        "standalone": "false",
        "verbose": "false",
        "botRestart": "0",
        "sleep": "15"
    }
}
```
For More Details Please Visit The [Wiki](https://github.com/AtsutaneDotNet/LickHunterPro-Assistant/wiki/LickHunterPro-Assistant-wiki!)

## Credits
- [LickHunterPro](https://github.com/CryptoGnome/LickHunterPRO) By [CryptoGnome](https://github.com/CryptoGnome)
- [LickHunterPro Variable Pairs](https://github.com/doosjenever/Scripts) By [doosjenever](https://github.com/doosjenever)
- Free Robot Icon By [Icongeek26](https://www.flaticon.com/authors/icongeek26)

## Donate To LickHunterPro-Assistant Development
- **ETH/BSC** 0xaD687b24852Ae916Cfb740871768E7b214175729
