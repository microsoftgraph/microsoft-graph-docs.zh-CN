---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aecb46a101b3e3f30c3b5e840747ed236cc346b77401bd430ec943ba6f057eaa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161967"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: 'Meet for lunch?',
    body: {
      contentType: 'Text',
      content: 'The new cafeteria is open.'
    },
    toRecipients: [
      {
        emailAddress: {
          address: 'fannyd@contoso.onmicrosoft.com'
        }
      }
    ],
    ccRecipients: [
      {
        emailAddress: {
          address: 'danas@contoso.onmicrosoft.com'
        }
      }
    ]
  },
  saveToSentItems: 'false'
};

await client.api('/me/sendMail')
    .post(sendMail);

```