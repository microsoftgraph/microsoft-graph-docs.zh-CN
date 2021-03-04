---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6a46cf854c10799313c542793cdb8716d870de0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/15d889df-3eb8-4e9b-bfb4-b1908849aec4/accessPackageResourceRoles')
    .version('beta')
    .filter('(originSystem eq \'AadGroup\' and accessPackageResource/id eq \'a35bef72-a8aa-4ca3-af30-f6b2ece7208f\')')
    .expand('accessPackageResource/id%20eq%20\'a35bef72-a8aa-4ca3-af30-f6b2ece7208f\')')
    .get();

```