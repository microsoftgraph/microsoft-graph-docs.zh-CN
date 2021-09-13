---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e6745068b3812e9330facd17184604a89ec7641eb878b5d5633f84944679bdec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218762"
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