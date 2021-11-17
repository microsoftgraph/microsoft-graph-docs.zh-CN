---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e897febdb947cacfde5ba05772ce6bb1230d609293abc07eea205e0430dc44f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221368"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: 'Annual review',
  body: {
    contentType: 'HTML',
    content: 'You should be proud!'
  },
  toRecipients: [
    {
      emailAddress: {
        address: 'rufus@contoso.com'
      }
    }
  ],
  extensions: [
    {
      '@odata.type': 'microsoft.graph.openTypeExtension',
      extensionName: 'Com.Contoso.Referral',
      companyName: 'Wingtip Toys',
      expirationDate: '2015-12-30T11:00:00.000Z',
      dealValue: 10000
    }
  ]
};

await client.api('/me/messages')
    .version('beta')
    .post(message);

```