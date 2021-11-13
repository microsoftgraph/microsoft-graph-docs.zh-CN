---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06ab37ea24b948b21f08126807a2fc8eaa237d7f
ms.sourcegitcommit: c6a8c1cc13ace38d6c4371139ee84707c5c93352
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2021
ms.locfileid: "60890646"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const markChatReadForUser = {
 user: {
    id: 'd864e79f-a516-4d0f-9fee-0eeb4d61fdc2'
  },
  tenantId: '2a690434-97d9-4eed-83a6-f5f13600199a'
};

await client.api('/chats/19:7d898072-792c-4006-bb10-5ca9f2590649_8ea0e38b-efb3-4757-924a-5f94061cf8c2@unq.gbl.spaces/markChatReadForUser')
    .version('beta')
    .post(markChatReadForUser);

```