---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dbc7a193353aca0d3b845c849e420e67f0be9113
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    roles: [],
    'user@odata.bind': 'https://graph.microsoft.com/beta/users/24b3819b-4e1d-4f3e-86bd-e42b54d0b2b4'
};

await client.api('/teams/6a720ba5-7373-463b-bc9f-4cd04b5c6742/channels/19:LpxShHZZh9utjNcEmUS5aOEP9ASw85OUn05NcWYAhX81@thread.tacv2/members')
    .version('beta')
    .post(conversationMember);

```