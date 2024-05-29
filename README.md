# Widgets Library

Update :

We just need to populate the imgUrl in the new widgets.json now as we read from [here](https://pro.openbb.co/assets/data/widgets.json) - The images can go in any of the folders above

Deprecated :

This repository contains the widget images that are going to be part of the Terminal Pro widget library documentation [here](https://docs.openbb.co/pro/widgets-library).

The [latest widgets.json file](https://github.com/OpenBB-finance/terminalpro/blob/colinsmh/src/lib/widgets.json) on the Terminal Pro should be copy-pasted to the root of this repo.

This is what will be used to get the `category`, `widgetId`, `name`, `description`, and `source`.

The widgets.json file will have the following format:

```json
"market_overview": {
  "searchCategory": "general-information",
  "name": "Market Indices",
  "description": "Show market overview (SP500, Nasdaq, Gold, ...)",
  "category": "equity",
  "widgetType": "individual",
  "widgetId": "market_overview",
  "gridData": {
    "w": 40,
    "h": 2,
    "minW": 20
  },
  "source": [
    "fmp"
  ]
},
"equity_select": {
  "searchCategory": "price",
  "name": "Ticker Information",
  "description": "Ticker Information",
  "category": "equity",
  "widgetType": "individual",
  "widgetId": "equity_select",
  "gridData": {
    "w": 20,
    "h": 2
  },
  "source": [
    "fmp"
  ]
},
```

An image needs to be created in this repository with the following format: {category}/{widgetId}.png.

This is what will be used to generate the docs images.
