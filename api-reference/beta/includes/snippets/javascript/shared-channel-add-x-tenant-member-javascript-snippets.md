---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 206ce2fe6f92b4bf65fdaf14a8283aab72da54bb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    roles: [],
    'user@odata.bind': 'https://graph.microsoft.com/beta/users/bc3598dd-cce4-4742-ae15-173429951408',
    tenantId: 'a18103d1-a6ef-4f66-ac64-e4ef42ea8681'
};

await client.api('/teams/6a720ba5-7373-463b-bc9f-4cd04b5c6742/channels/19:LpxShHZZh9utjNcEmUS5aOEP9ASw85OUn05NcWYAhX81@thread.tacv2/members')
    .version('beta')
    .post(conversationMember);

```