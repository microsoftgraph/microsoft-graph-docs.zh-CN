---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1fce0ffcf747890ca648176dff543cc2a765783
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581081"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5',
    roles: ['owner']
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .post(conversationMember);

```