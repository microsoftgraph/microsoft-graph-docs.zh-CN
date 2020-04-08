---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fa4083cb94b86397ac1c5fd6a16f521f663fa4a
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181158"
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
    directoryScopeId: "5d107bba-d8e2-4e13-b6ae-884be90e5d1a" //object id of an administrative unit
};

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```