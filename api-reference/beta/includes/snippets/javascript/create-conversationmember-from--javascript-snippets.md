---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edfa1240c77d2e09f1fd527d715a7cd0f644139d
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45080900"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    @odata.type: "#microsoft.graph.aadUserConversationMember",
    roles: [
        "owner"
    ],
    userId: "50dffbae-ad0f-428e-a86f-f53b0acfc641",
    displayName: "Cameron White",
    email: "CameronW@M365x987948.OnMicrosoft.com"
};

let res = await client.api('/teams/{id}/members')
    .version('beta')
    .post(conversationMember);

```