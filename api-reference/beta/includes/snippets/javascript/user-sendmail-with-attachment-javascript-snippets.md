---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aa033cd5becec64a48f9881b13d217d7ddf436f
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774446"
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
    .version('beta')
    .post(sendMail);

```