---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3220b890310b0286158258babc648a2a2cef7e9a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799524"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRoleScope = {
  accessPackageResourceRole: {
    originId: 'Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca',
    displayName: 'Member',
    originSystem: 'AadGroup',
    accessPackageResource: {id: '1d08498d-72a1-403f-8511-6b1f875746a0',resourceType: 'O365 Group',originId: 'b31fe1f1-3651-488f-bd9a-1711887fd4ca',originSystem: 'AadGroup'}
  },
 accessPackageResourceScope: {
   originId: 'b31fe1f1-3651-488f-bd9a-1711887fd4ca',originSystem: 'AadGroup'
 }
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes')
    .version('beta')
    .post(accessPackageResourceRoleScope);

```