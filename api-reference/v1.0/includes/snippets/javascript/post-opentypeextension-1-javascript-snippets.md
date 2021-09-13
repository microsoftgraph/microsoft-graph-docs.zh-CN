---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3f87118ad56557afede350f8b850bf39845d56228cd157b7e89603eda66ca070
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277665"
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