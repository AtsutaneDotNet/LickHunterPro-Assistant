# LickHunterPro-Assistant
Assistant Software to manage LickHunterPro Bot using python and liquidation data from https://liquidation.atsutane.net

![LHPA-UI](https://user-images.githubusercontent.com/6040550/121283129-33751100-c90d-11eb-8435-93f81acf2bfd.PNG)
![LHA-Webhook](https://user-images.githubusercontent.com/6040550/121284778-f6f6e480-c90f-11eb-965c-1c0d0cab4177.PNG)
![LHA-Menu](https://user-images.githubusercontent.com/6040550/121283197-4f78b280-c90d-11eb-8483-cc99fd1ac573.PNG)

# LickHunterPro-Assistant Features
- [x] Automatically choose pairs for trading base from balance, leverage and percentBal
- [x] Automatically choose lick value, long offset & short offset base on data from https://liquidation.atsutane.net
- [x] Discord Webhook support for notification and status change
- [x] Automatically transfer balance from future to spot.
- [x] Support using secondary take profit value when reach isolation mode.
- [x] Support emergency exit plan by reducing secondary take profit value into half when margin is over 50%
- [x] Interactive hotkey menu
- [x] Colorfull discord embed :D
- [ ] still building the list

# LickHunterPro-Assistant Setup
Just change *control.json* suitable to your need and run *LickHunterAssistant.exe*
```json
{
    "tradingSettings": {
        "maxPairs": "100",
        "maxPositions": "5",
        "IsoPercentage": "10",
        "PrimaryProfit": "1.06",
        "SecondaryProfit": "0.795",
        "EmergencyExit": "false",
        "EmergencyTrigger": "25",
        "EmergencyProfit": "0.5"
    },
    "tradingPairs": {
        "CurrentPairs": "",
        "LastUsedPairs": "",
        "blacklist": ""
    },
    "tradingAI": {
        "autoPbal": "true",
        "autoMaxPos": "true",
        "LickValueType": "mean",
        "MaxPerPos": "400",
        "nominalValue": "6",
        "MaxMin": "false",
        "maxVwap": "8",
        "minVwap": "4"
    },
    "autoTransfer": {
        "status": "false",
        "limit": "1000",
        "percentage": "10"
    },
    "misc": {
        "standalone": "false",
        "verbose": "false",
        "webHookDelay": "1200",
        "sleep": "15"
    }
}
```
For More Details Please Visit The [Wiki](https://github.com/AtsutaneDotNet/LickHunterPro-Assistant/wiki/LickHunterPro-Assistant-wiki!)

# Credits
- [LickHunterPro](https://github.com/CryptoGnome/LickHunterPRO) By [CryptoGnome](https://github.com/CryptoGnome)
- [LickHunterPro Variable Pairs](https://github.com/doosjenever/Scripts) By [doosjenever](https://github.com/doosjenever)
- Free Robot Icon By [Icongeek26](https://www.flaticon.com/authors/icongeek26)

# Donate To LickHunterPro-Assistant Development
- **ETH/BSC** 0xaD687b24852Ae916Cfb740871768E7b214175729
