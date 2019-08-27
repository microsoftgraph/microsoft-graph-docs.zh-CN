---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c69ccfcc7db58b2ddf79abb4048bc39274eaa00e
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636716"
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
    .post(conversation);

```