---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76460a1f0f7e0efedd0f92ed7dc2213c19386677a429fa78dd8576f743b81843
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161644"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
    subject: 'Party planning',
    toRecipients: [
      {
          emailAddress: {
              name: 'Samantha Booth',
              address: 'samanthab@contoso.onmicrosoft.com'
          }
      }
    ],
    mentions: [
      {    
        mentioned: {
          name: 'Dana Swope',
          address: 'danas@contoso.onmicrosoft.com'
         }
      }
    ]
};

await client.api('/me/messages')
    .version('beta')
    .post(message);

```