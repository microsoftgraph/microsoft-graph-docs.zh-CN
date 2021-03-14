---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 444547e70a3ab00f6647139d258d38eff4fa3329
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803261"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  '@odata.type':'#Microsoft.OutlookServices.ConversationThread',
  isLocked: true
};

await client.api('/groups/{id}/threads/{id}')
    .update(conversationThread);

```