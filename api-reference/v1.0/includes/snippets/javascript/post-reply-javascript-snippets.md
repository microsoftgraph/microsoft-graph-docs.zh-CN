---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4de519839c8b488a4a6d41dedbf16826bd0d7683
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783393"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: '',
      content: 'content-value'
    },
    receivedDateTime: 'datetime-value',
    hasAttachments: true,
    from: {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    },
    sender: {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    },
    conversationThreadId: 'conversationThreadId-value',
    newParticipants: [
      {
        emailAddress: {
          name: 'name-value',
          address: 'address-value'
        }
      }
    ],
    conversationId: 'conversationId-value',
    createdDateTime: 'datetime-value',
    lastModifiedDateTime: 'datetime-value',
    changeKey: 'changeKey-value',
    categories: [
      'categories-value'
    ],
    id: 'id-value',
    inReplyTo: {
    },
    attachments: [
      {
        '@odata.type': '#microsoft.graph.fileAttachment',
        lastModifiedDateTime: 'datetime-value',
        name: 'name-value',
        contentType: 'contentType-value',
        size: 99,
        isInline: true,
        id: 'id-value'
      }
    ]
  }
};

await client.api('/groups/{id}/threads/{id}/posts/{id}/reply')
    .post(reply);

```