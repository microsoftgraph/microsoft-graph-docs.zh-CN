---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d0ec590af3d1ebbb4a765565199942d7725b0c93
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453563"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: "New Conversation Thread Topic",
  posts: [{
    body: {
      contentType: "html",
      content: "this is body content"
    },
    newParticipants: [{
      emailAddress: {
        name: "Alex Darrow",
        address: "alexd@contoso.com"
      }
    }]
  }]
};

let res = await client.api('/groups/{id}/threads')
    .version('beta')
    .post({conversationThread : conversationThread});

```