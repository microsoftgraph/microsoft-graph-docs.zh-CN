---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a41a7d08ab99712b3ddf1d919e8b3abc3dede4a
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206984"
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
    .post(unifiedRoleAssignment);

```