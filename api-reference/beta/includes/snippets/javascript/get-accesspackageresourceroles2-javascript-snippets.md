---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ade932a850d3c581be3cefd01cc7b17024f7516e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439246"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResourceRoles = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/beedadfe-01d5-4025-910b-84abb9369997/accessPackageResourceRoles')
    .version('beta')
    .filter('(originSystem eq \'SharePointOnline\' and accessPackageResource/id eq \'53c71803-a0a8-4777-aecc-075de8ee3991\')')
    .select('displayName,originId')
    .get();

```