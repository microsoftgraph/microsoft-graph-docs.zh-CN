---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a040b5a8e704ff19fde0a643e059b5e1eecaf05
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799829"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: 'html',
      content: '<html><body><div><div><div><div>When and where? </div></div></div></div></body></html>'
    },
  extensions: [
    {
      '@odata.type': 'microsoft.graph.openTypeExtension',
      extensionName: 'Com.Contoso.HR',
      companyName: 'Contoso',
      expirationDate: '2015-07-03T13:04:00.000Z',
      topPicks: [
        'Employees only',
        'Add spouse or guest',
        'Add family'
      ]
    }
  ]
  }
};

await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/threads/AAQkADJizZJpEWwqDHsEpV_KA==/posts/AAMkADJiUg96QZUkA-ICwMubAAC1heiSAAA=/reply')
    .version('beta')
    .post(reply);

```