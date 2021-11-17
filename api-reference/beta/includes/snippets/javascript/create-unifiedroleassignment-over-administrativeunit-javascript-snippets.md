---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f9f668419bdcc634c03966f4ae259d07af3ffb65084197e1a57ca810b14a3fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106868"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignment',
    roleDefinitionId: 'fe930be7-5e62-47db-91af-98c3a49a38b1', //template id of User Account Administrator
    principalId: 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d',
    directoryScopeId: '/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a' //object id of an administrative unit
};

await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```