---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e100420903fa612b2be7573e30a92f93c5abbab8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470878"
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
    .post(reply);

```