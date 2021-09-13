---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 20415d21e289428ce5ac95a61e371afa19d3e738c8d85d147f131eeac0da3b69
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277666"
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
    .post(conversation);

```