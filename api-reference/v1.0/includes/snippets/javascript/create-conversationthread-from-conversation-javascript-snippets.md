---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2802fb6dfa7bd4cdd15dcb524ccf5163d05d8cedab9fde9383201a4292c8ed3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332633"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: 'topic-value',
  posts: [{
      body: {
        contentType: 'html',
        content: 'this is body content'
      }
  }]
};

await client.api('/groups/{id}/conversations/{id}/threads')
    .post(conversationThread);

```