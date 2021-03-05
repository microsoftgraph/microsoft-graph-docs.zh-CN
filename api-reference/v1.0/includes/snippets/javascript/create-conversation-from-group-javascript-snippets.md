---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d9d1c225a35cd0ae1268ef3796206306a1fb616
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversation = {
  topic: 'New locations for this quarter',
  threads: [
    {
      posts: [
        {
          body: {
            contentType: 'html',
            content: 'What do we know so far?'
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
    .post(conversation);

```