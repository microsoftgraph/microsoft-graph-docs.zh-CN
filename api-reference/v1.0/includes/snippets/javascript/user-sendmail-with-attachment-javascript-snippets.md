---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb8edb0b38427a082a98aab0fd9a4c743164143f7104500c98f3099cebcbca04
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215940"
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