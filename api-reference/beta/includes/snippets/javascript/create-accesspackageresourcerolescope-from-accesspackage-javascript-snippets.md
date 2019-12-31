---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3a9c17a0397c80242b6de742c2ad491fe0a3f39
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageResourceRoleScope = {
  accessPackageResourceRole:{
    originId:"Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
    displayName:"Member",
    originSystem:"AadGroup",
    accessPackageResource:{id:1d08498d-72a1-403f-8511-6b1f875746a0","resourceType:O365 Group","originId:b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem:"AadGroup"}
  },
 accessPackageResourceScope:{
   originId:b31fe1f1-3651-488f-bd9a-1711887fd4ca","originSystem:"AadGroup"
 }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackageResourceRoleScopes')
    .version('beta')
    .post(accessPackageResourceRoleScope);

```