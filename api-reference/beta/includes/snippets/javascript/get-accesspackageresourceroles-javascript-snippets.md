---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbdc4a52e89fa3653dc0e10b78aeaeb3e7553b16820a14db6fdd3a88a794d782
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902775"
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