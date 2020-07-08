---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46077d0107d43d5096b40bfd6bdb7c6527951445
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081721"
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
    appScopeIds: ["allDevices"]
};

let res = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignmentMultiple);

```