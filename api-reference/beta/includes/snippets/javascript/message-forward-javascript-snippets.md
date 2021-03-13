---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed510ea8c301dd224879433991386ac23bc36d9d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  message: {  
    isDeliveryReceiptRequested: true,
    toRecipients: [
      {
        emailAddress: {
          address: 'danas@contoso.onmicrosoft.com',
          name: 'Dana Swope'
        }
      }
     ]
  },
  comment: 'Dana, just want to make sure you get this.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/forward')
    .version('beta')
    .post(forward);

```