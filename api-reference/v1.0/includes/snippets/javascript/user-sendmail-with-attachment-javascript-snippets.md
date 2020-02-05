---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c0a5867e45f8067d4b2fbf657f7a2485ff758a9
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774350"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: "Meet for lunch?",
    body: {
      contentType: "Text",
      content: "The new cafeteria is open."
    },
    toRecipients: [
      {
        emailAddress: {
          address: "meganb@contoso.onmicrosoft.com"
        }
      }
    ],
    attachments: [
      {
        @odata.type: "#microsoft.graph.fileAttachment",
        name: "attachment.txt",
        contentType: "text/plain",
        contentBytes: "SGVsbG8gV29ybGQh"
      }
    ]
  }
};

let res = await client.api('/me/sendMail')
    .post(sendMail);

```