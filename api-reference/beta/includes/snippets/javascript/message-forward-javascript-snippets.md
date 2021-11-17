---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 247006975c5648d29dde241248494912e3413f1a69ec10cc6791b5301f5342d8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221319"
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