---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b98b983140ce29e1a199e6647f7587c8557f2c0aabb952f4a74702b84668cd81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221369"
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