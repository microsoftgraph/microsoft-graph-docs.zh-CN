---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9aac35f758a3154b95db2d64803fe80c442df37e
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314446"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    @odata.type: "#microsoft.graph.aadUserConversationMember",
    roles: ["owner"],
    user@odata.bind: "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"
};

let res = await client.api('/teams/{id}/members')
    .post(conversationMember);

```