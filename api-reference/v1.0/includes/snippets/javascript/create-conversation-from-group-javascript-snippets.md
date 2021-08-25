---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b797f4982811809aa626155870ca25a80ed2d5f7f4a60e60fe5eeef30f25147
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106796"
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