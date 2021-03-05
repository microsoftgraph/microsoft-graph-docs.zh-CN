---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 575f1a4f0d9dfab0795a748b0c60a0513303f852
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470862"
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
    .post(message);

```