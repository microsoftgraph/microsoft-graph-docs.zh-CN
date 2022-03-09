---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6da3f8a6790c62ec5d673cfdd9626113a7d961fb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396509"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/entitlementManagement/roleAssignments')
    .version('beta')
    .filter('appScopeId eq \'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc\'')
    .expand('principal')
    .get();

```