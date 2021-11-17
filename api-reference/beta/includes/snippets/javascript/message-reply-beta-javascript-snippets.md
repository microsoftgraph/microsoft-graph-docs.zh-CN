---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 267270a6caac2cb8d2739bde0b7fd53e3e76dbe20fb2da24d0934a32b780d545
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333108"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  message: {  
    toRecipients: [
      {
        emailAddress: {
          address: 'samanthab@contoso.onmicrosoft.com',
          name: 'Samantha Booth'
        }
      },
      {
        emailAddress: {
          address: 'randiw@contoso.onmicrosoft.com',
          name: 'Randi Welch'
        }
      }
     ]
  },
  comment: 'Samantha, Randi, would you name the group please?' 
};

await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/reply')
    .version('beta')
    .post(reply);

```