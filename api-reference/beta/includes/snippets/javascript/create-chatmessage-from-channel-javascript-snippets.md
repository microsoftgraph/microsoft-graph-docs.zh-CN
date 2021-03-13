---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 43a34d286865d9d402547bec1cf09a5b6fbbf8d6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801617"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    content: 'Hello World'
  }
};

await client.api('/teams/{id}/channels/{id}/messages')
    .version('beta')
    .post(chatMessage);

```