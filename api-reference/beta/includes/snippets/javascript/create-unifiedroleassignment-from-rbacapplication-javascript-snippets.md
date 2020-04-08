---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 070b70b77ae9a7008e5afc4779e01ba7e389a72b
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    @odata.type: "#microsoft.graph.unifiedRoleAssignment",
    roleDefinitionId: "c2cf284d-6c41-4e6b-afac-4b80928c9034",
    principalId: "f8ca5a85-489a-49a0-b555-0a6d81e56f0d",
    directoryScopeId: "/"
};

let res = await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```