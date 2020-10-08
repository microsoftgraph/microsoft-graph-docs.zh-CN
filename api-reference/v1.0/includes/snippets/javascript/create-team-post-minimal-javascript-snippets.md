---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1137088c27ed3fb07831c56fc71f78519e99333a
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/07/2020
ms.locfileid: "48374062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const team = {
  template@odata.bind: "https://graph.microsoft.com/v1.0/teamsTemplates('standard')",
  displayName: "My Sample Team",
  description: "My Sample Team’s Description",
  members@odata.bind: [
            {
            @odata.type: "#microsoft.graph.aadUserConversationMember",
            roles: ["owner"],
            userId: "0040b377-61d8-43db-94f5-81374122dc7e"
        }
  ]
};

let res = await client.api('/teams')
    .post(team);

```