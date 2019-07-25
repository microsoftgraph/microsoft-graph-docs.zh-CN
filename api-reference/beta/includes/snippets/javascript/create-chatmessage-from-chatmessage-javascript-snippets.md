---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6d3fbab98af09ce3d5edbb86a42c39a892098dcb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     "content" : "Hello world"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages/{id}/replies')
    .version('beta')
    .post({chatMessage : chatMessage});

```