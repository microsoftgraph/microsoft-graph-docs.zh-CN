---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac0d7c7445b0618dba02f455f09f82904f4b5eb8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808066"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5'
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .version('beta')
    .post(conversationMember);

```