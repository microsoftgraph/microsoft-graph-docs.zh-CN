---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 10828745f5c514ec625daf362771bd55ad2379f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    roles: ['owner'],
    'user@odata.bind': 'https://graph.microsoft.com/v1.0/users(\'8b081ef6-4792-4def-b2c9-c363a1bf41d5\')'
};

await client.api('/teams/ece6f0a1-7ca4-498b-be79-edf6c8fc4d82/channels/19:56eb04e133944cf69e603c5dac2d292e@thread.skype/members')
    .version('beta')
    .post(conversationMember);

```