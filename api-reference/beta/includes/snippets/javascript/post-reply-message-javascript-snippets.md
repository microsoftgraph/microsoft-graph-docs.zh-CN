---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31d04c8ebca9b1f709bc93a8092ff32e509ae937
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479225"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    contentType: "html",
    content: "Hello World"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages/{id}/replies')
    .version('beta')
    .post({chatMessage : chatMessage});

```