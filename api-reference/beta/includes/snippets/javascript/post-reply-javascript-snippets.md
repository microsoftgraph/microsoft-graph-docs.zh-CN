---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fff83f61f05dd4da15e807a2d8c1a0c900f2ec2eb71f9473c57d7a0d5fcb211e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902492"
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
    receivedDateTime: '2016-10-19T10:37:00Z',
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
    createdDateTime: '2016-10-19T10:37:00Z',
    lastModifiedDateTime: '2016-10-19T10:37:00Z',
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
        lastModifiedDateTime: '2016-10-19T10:37:00Z',
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
    .version('beta')
    .post(reply);

```