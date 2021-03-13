---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66e2c62a71961e76cfbf7d02f4be8afabfad03da
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
  Topic: 'Does anyone have a second?',
  Threads: [
    {
      Posts: [
        {
          Body: {
            ContentType: 'HTML',
            Content: 'This is urgent!'
          },
          Extensions: [
            {
              '@odata.type': 'microsoft.graph.openTypeExtension',
              extensionName: 'Com.Contoso.Benefits',
              companyName: 'Contoso',
              expirationDate: '2016-08-03T11:00:00.000Z',
              topPicks: [
                'Employees only',
                'Add spouse or guest',
                'Add family'
              ]
            }
          ]
        }
      ]
    }
  ]
};

await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations')
    .version('beta')
    .post(conversation);

```