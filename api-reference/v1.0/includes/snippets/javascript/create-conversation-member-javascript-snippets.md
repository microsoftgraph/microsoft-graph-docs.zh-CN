---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a73ff2e580c647d6e1c5568ce7126cc941620bda0b7f37ec6c31b903147d9b2c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902990"
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