---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d4d65744da49db036913dfa9bd8edfc607db04e
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48619187"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "",
      content: "content-value"
    },
    receivedDateTime: "datetime-value",
    hasAttachments: true,
    from: {
      emailAddress: {
        name: "name-value",
        address: "address-value"
      }
    },
    sender: {
      emailAddress: {
        name: "name-value",
        address: "address-value"
      }
    },
    conversationThreadId: "conversationThreadId-value",
    newParticipants: [
      {
        emailAddress: {
          name: "name-value",
          address: "address-value"
        }
      }
    ],
    conversationId: "conversationId-value",
    createdDateTime: "datetime-value",
    lastModifiedDateTime: "datetime-value",
    changeKey: "changeKey-value",
    categories: [
      "categories-value"
    ],
    id: "id-value",
    inReplyTo: {
    },
    attachments: [
      {
        lastModifiedDateTime: "datetime-value",
        name: "name-value",
        contentType: "contentType-value",
        size: 99,
        isInline: true,
        id: "id-value"
      }
    ]
  }
};

let res = await client.api('/groups/{id}/threads/{id}/posts/{id}/reply')
    .post(reply);

```