---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1a353275b11ba16c92aebea66405459b8c44651f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788846"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignment',
    roleDefinitionId: 'c2cf284d-6c41-4e6b-afac-4b80928c9034',
    principalId: 'f8ca5a85-489a-49a0-b555-0a6d81e56f0d',
    directoryScopeId: '/'
};

await client.api('/roleManagement/directory/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```