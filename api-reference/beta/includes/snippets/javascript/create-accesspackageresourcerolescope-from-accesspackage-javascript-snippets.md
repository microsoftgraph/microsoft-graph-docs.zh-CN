---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f9733cb19cf719dd9a60a2b835c91ba66e01130b41e653d936dcf57a0acee02
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902829"
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