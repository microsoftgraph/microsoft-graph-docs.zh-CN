---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0d9171336904a57bda1c76d229f299a3d5373364
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636549"
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

let res = await client.api('/teams/{id}/channels/{id}/messages')
    .version('beta')
    .post(chatMessage);

```