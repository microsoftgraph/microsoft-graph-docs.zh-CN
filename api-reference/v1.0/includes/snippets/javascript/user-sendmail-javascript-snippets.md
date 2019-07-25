---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 988f23fdbf5df753773d021bad7b9af5e5a12c9f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711398"
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
          address: "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    ccRecipients: [
      {
        emailAddress: {
          address: "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  saveToSentItems: "false"
};

let res = await client.api('/me/sendMail')
    .post(sendMail);

```