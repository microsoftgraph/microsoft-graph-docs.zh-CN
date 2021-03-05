---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 29939a0cf34718505e5f17aa89396c9b15747402
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
  topic: 'New head count',
  threads: [
    {
      posts: [
        {
          body: {
            contentType: 'html',
            content: 'The confirmation will come by the end of the week.'
          },
          newParticipants: [
            {
              emailAddress: {
                name: 'Adele Vance',
                address: 'AdeleV@contoso.onmicrosoft.com'
              }
            }
          ]
        }
      ]
    }
  ]
};

await client.api('/groups/29981b6a-0e57-42dc-94c9-cd24f5306196/conversations')
    .version('beta')
    .post(conversation);

```