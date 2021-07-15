---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b69ffb89ab421f0bccc4b85842505b54880704e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442191"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignment = {
    principalId: '679a9213-c497-48a4-830a-8d3d25d94ddc',
    roleDefinitionId: 'ae79f266-94d4-4dab-b730-feca7e132178',
    appScopeId: '/AccessPackageCatalog/beedadfe-01d5-4025-910b-84abb9369997'
};

await client.api('/roleManagement/entitlementManagement/roleAssignments')
    .version('beta')
    .post(unifiedRoleAssignment);

```