---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 97b3a38f4b05fb979b5cd154c1622f878db912fb
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581332"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResources = await client.api('/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources')
    .version('beta')
    .filter('resourceType eq \'Application\'')
    .expand('accessPackageResourceScopes')
    .get();

```