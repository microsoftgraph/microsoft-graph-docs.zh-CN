---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4bff9e8c6ea3d2c9eb280dbf06a7eabb13be25c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786012"
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
    .post(reply);

```