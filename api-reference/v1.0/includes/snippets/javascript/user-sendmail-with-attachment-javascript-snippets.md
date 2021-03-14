---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b89ba8c3285b43d907727215e7f8ebc810d641e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800239"
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
          address: 'meganb@contoso.onmicrosoft.com'
        }
      }
    ],
    attachments: [
      {
        '@odata.type': '#microsoft.graph.fileAttachment',
        name: 'attachment.txt',
        contentType: 'text/plain',
        contentBytes: 'SGVsbG8gV29ybGQh'
      }
    ]
  }
};

await client.api('/me/sendMail')
    .post(sendMail);

```