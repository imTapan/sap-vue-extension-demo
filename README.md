# sap-vue-extension-demo

Vue App Demo for SAP Web Client Extension

## Steps to integrate

- Take Clone, it's Public 😃
- Put Required ENV & Run as Dev mode for check.
- Generate Build & Use Build Files as Extension
- & Done.

#### After Build Setup

- Make `WebClientExtension.json` in Dist Folder & put code

```js
{
  "tiles": [
    {
      "text": "vue-app-webclient",
      "icon": "sap-icon://customize",
      "url": "index.html",
      "subtitle": "Web Client Vue Application Extension"
      "size": "1x1",
      "dynamicContent": {
        "repositories": [
          {
            "converter": "kpiNumber",
            "endpoint": "/b1s/v2/PurchaseOrders/$count"
          }
        ]
      }
    }
  ]
}
```

- Next Command :`mbt build`
