---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fbf8198d1a019114a6d61f6b7a0fa30d71c9396c0b1aa9e68aa5797ab8c4cdec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902774"
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