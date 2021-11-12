---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05e9c62a7787c4c751fe3ce874c5d51e70d102d5ad76b6825145c8e8983120cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277739"
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
    .version('beta')
    .post(sendMail);

```