---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: 0dab31dd01554d72ac6dd78aff604a6ead55f2c9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49350444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     content: "Hello world"
  }
};

let res = await client.api('/teams/{id}/channels/{id}/messages')
    .version('beta')
    .post(chatMessage);

```