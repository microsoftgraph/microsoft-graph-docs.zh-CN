---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 57275718a6a7acda0c0cce5f619c16a2ccd1794766bfef80f06c92a2780e1cdf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57219321"
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