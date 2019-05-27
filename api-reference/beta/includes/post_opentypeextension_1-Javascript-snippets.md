---
description: 自动生成的文件。 不修改
ms.openlocfilehash: aedee0f168d83cacc6a98178351d9b2428ed7b9c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443423"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: "Annual review",
  body: {
    contentType: "HTML",
    content: "You should be proud!"
  },
  toRecipients: [
    {
      emailAddress: {
        address: "rufus@contoso.com"
      }
    }
  ],
  extensions: [
    {
      @odata.type: "microsoft.graph.openTypeExtension",
      extensionName: "Com.Contoso.Referral",
      companyName: "Wingtip Toys",
      expirationDate: "2015-12-30T11:00:00.000Z",
      dealValue: 10000
    }
  ]
};

let res = await client.api('/me/messages')
    .version('beta')
    .post({message : message});

```