---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2fd9e0c8df041e425aa6f80293c67ecbb0582a53
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59061031"
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
    .post(unifiedRoleAssignment);

```