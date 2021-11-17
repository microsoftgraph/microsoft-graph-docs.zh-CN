---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d443f8293908e9551ff7ddf03ef6e7ba9969538f903c84e3fad69c1864da8c4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277641"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     content: 'Hello world'
  }
};

await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .version('beta')
    .post(chatMessage);

```