# Wrapper for Payture widget

## 📦 Install

```
npm i mapayturewrapper
```

## 🛠️ Sample usage

```javascript
const payturewrapper = require('mapayturewrapper');
payturewrapper.loadDependencies();
payturewrapper.openWidget({
      Key : "Merchant_Widget",
      Amount : 1000,
      Product : "Service payment",
      Domain : 2,
      CustomParams :{TemplateTag : "Default",Language : "ENG"},
      ChequeParams :{Positions:[{Quantity: 1.000,Price: 1000.00,Text: "Service"}],CustomerContact : "",Message: "Cheque Payture for Service"},
      OnTransactionCompleted : function(success) {alert( success );}
    });
```

## 🔗 [Payture Offical Docs](https://payture.com/en/api/#widget-docs_)