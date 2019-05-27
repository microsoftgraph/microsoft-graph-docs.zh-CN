---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a68dd0c10d2886dfba47de87a1a191a1da6176fd
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439867"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  userId: "userId-value",
  roleId: "roleId-value"
};

let res = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .post({privilegedRoleAssignment : privilegedRoleAssignment});

```