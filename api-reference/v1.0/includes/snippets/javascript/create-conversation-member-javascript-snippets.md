---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b330fb0bfa0fd53f0c1e3169bfb1cac5908523b4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  '@odata.type': '#microsoft.graph.aadUserConversationMember',
  roles: [],
  'user@odata.bind': 'https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5'
};

await client.api('/teams/{id}/channels/{id}/members/')
    .post(conversationMember);

```