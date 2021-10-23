---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34b3ba7483014f260fe9acc5a64f5fd6d1e49ec2c6476cda99b53c016f3f315c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106361"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5',
    visibleHistoryStartDateTime: '0001-01-01T00:00:00Z',
    roles: ['owner']
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .version('beta')
    .post(conversationMember);

```