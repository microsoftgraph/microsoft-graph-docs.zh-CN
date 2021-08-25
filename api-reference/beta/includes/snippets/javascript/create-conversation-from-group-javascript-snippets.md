---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0f3f16bc54c89a7a729ba87b976dfb4dc573eff42ca3fb4af911366abcf98d7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219210"
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