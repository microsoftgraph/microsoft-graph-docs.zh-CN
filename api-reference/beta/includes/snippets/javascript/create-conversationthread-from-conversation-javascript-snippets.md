---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 930f9c40093a752a07aef6b7fd9da8196f9ae55b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636543"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: "topic-value",
  posts: [{
      body: {
        contentType: "html",
        content: "this is body content"
      }
  }]
};

let res = await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .post(conversationThread);

```