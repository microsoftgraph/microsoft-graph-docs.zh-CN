---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d4d65744da49db036913dfa9bd8edfc607db04e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739603"
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