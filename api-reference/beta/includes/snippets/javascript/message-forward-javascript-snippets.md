---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff47ebac31ccbcd132bafb64dcece94bd724edae
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "35729716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  message:{  
    isDeliveryReceiptRequested: true,
    toRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ]
  },
  comment: "Dana, just want to make sure you get this." 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward')
    .version('beta')
    .post(forward);

```