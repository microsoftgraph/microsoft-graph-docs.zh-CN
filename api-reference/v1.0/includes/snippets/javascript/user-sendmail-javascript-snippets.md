---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2131cda902ded9046e9bd614d9816d4c355b199
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803624"
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