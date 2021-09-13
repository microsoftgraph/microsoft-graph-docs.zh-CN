---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d801371739a57b80d4e90f9e92c27c55e2c86f2996d40b25ea2aa88524f7cc8c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903373"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5',
    visibleHistoryStartDateTime: '2019-04-18T23:51:43.255Z',
    roles: ['owner']
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .post(conversationMember);

```