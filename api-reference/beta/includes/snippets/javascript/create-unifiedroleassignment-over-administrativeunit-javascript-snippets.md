---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0abd3d8c79d060e453efbbe6a657000a1d8ffd34
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44794484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    @odata.type: "#microsoft.graph.unifiedRoleAssignment",
    roleDefinitionId: "fe930be7-5e62-47db-91af-98c3a49a38b1", //template id of User Account Administrator
    principalId: "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    directoryScopeId: "/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
};

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```