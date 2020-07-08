---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f308dfb76fa2e42efd650be68e0f856d45eb4173
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081720"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    @odata.type: "#microsoft.graph.unifiedRoleAssignmentMultiple",
    displayName: "My test role assignment 1",
    roleDefinitionId: "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    principalIds: ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    directoryScopeIds: ["28ca5a85-489a-49a0-b555-0a6d81e56f0d", "8152656a-cf9a-4928-a457-1512d4cae295"],
};

let res = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignmentMultiple);

```