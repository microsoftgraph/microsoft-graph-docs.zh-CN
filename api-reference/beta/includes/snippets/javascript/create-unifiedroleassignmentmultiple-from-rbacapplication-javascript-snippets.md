---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec5d7f18e4458b68d5ead13517cfc2c6ab3ea6f99ce4077712dbf8c59f8ca45f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54274400"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    '@odata.type': '#microsoft.graph.unifiedRoleAssignmentMultiple',
    displayName: 'My test role assignment 1',
    roleDefinitionId: 'c2cf284d-6c41-4e6b-afac-4b80928c9034',
    principalIds: ['f8ca5a85-489a-49a0-b555-0a6d81e56f0d', 'c1518aa9-4da5-4c84-a902-a31404023890'],
    directoryScopeIds: ['28ca5a85-489a-49a0-b555-0a6d81e56f0d', '8152656a-cf9a-4928-a457-1512d4cae295'],
};

await client.api('/roleManagement/deviceManagement/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignmentMultiple);

```