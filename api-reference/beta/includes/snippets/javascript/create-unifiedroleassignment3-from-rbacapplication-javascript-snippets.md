---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8fc05b0848f56b4183dcbe7795c2f44f5e532ca43df319fb2e7d7d0b8bdc8055
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163208"
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