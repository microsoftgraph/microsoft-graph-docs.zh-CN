---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94906bd78ae493b66db2be7727ae34493edb3ddbcaa039701a20ecedbc22d08b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221374"
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