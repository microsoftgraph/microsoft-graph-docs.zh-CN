---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9035f29f5d56c7e4154802e39a58afa447bcfea7
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072362"
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
        @odata.type: "#microsoft.graph.fileAttachment",
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