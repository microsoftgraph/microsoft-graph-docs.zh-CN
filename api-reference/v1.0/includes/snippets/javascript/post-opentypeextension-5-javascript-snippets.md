---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65bf612c01bfec5612db26155fc0a114ac2c592b
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470882"
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