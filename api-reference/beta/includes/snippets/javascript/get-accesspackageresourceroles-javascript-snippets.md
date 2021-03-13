---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 383f27c450962a4450d3f042170367cdb90b3d81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778999"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResourceRoles = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles')
    .version('beta')
    .filter('(originSystem eq \'AadGroup\' and accessPackageResource/id eq \'a35bef72-a8aa-4ca3-af30-f6b2ece7208f\')')
    .expand('accessPackageResource/id%20eq%20\'a35bef72-a8aa-4ca3-af30-f6b2ece7208f\')')
    .get();

```