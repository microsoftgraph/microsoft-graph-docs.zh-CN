---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5f63772011fb6bb1f7f6af7f237b2d19a83321838369badd010e0b3cfa3dde5b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
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
  comment: 'Dana, just want to make sure you get this; you\'ll need this if the project gets approved.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward')
    .version('beta')
    .post(message);

```