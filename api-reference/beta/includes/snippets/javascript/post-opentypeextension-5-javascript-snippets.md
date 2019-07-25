---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 27c6319551c2c6f449fdc97b766538146bd25af6
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35729286"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
  Topic: "Does anyone have a second?",
  Threads: [
    {
      Posts: [
        {
          Body: {
            ContentType: "HTML",
            Content: "This is urgent!"
          },
          Extensions: [
            {
              @odata.type: "microsoft.graph.openTypeExtension",
              extensionName: "Com.Contoso.Benefits",
              companyName: "Contoso",
              expirationDate: "2016-08-03T11:00:00.000Z",
              topPicks: [
                "Employees only",
                "Add spouse or guest",
                "Add family"
              ]
            }
          ]
        }
      ]
    }
  ]
};

let res = await client.api('/groups/37df2ff0-0de0-4c33-8aee-75289364aef6/conversations')
    .version('beta')
    .post({conversation : conversation});

```