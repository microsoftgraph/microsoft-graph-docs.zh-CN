---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52b51f2fc2cf9f07ac36a03a813342e153fe18578288e1335bad3c0f1be20e5f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106359"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5',
    roles: ['owner']
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .version('beta')
    .post(conversationMember);

```