---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e8eb589ac80fc5e324f71dc617ba997b9aa108d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    @odata.type: "#microsoft.graph.unifiedRoleAssignmentMultiple",
    roleDefinitionId: "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    principalIds: ["f8ca5a85-489a-49a0-b555-0a6d81e56f0d", "c1518aa9-4da5-4c84-a902-a31404023890"],
    appScopeIds: ["allDevices"]
};

let res = await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignmentMultiple);

```