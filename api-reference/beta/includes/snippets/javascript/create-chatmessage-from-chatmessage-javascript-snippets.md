---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d75b99ebd4b3bdf2cad884554f04804fa11e29b0
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636548"
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
    .post(chatMessage);

```