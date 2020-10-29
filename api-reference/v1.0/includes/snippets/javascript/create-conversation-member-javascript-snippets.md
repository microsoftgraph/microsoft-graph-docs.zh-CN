---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 74ff2afea9baf2c03528941ad3d0f79c31d1e6ef
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  @odata.type: "#microsoft.graph.aadUserConversationMember",
  roles: [],
  user@odata.bind: "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
};

let res = await client.api('/teams/{id}/channels/{id}/members/')
    .post(conversationMember);

```