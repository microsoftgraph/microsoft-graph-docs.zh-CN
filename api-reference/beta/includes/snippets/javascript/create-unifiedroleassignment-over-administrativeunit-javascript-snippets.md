---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52948beff588678f1bbfebdc652813370ce330d7
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092699"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignment',
    roleDefinitionId: 'fe930be7-5e62-47db-91af-98c3a49a38b1',
    principalId: 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d',
    directoryScopeId: '/administrativeUnits/5d107bba-d8e2-4e13-b6ae-884be90e5d1a'
};

await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```