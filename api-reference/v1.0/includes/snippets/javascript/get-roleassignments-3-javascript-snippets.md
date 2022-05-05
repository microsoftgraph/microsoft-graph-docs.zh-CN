---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 102e8a98a5e21cfc2cf74f80506a2e0f465d6b03
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207437"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleAssignments = await client.api('/roleManagement/entitlementManagement/roleAssignments')
    .filter('appScopeId eq \'/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc\'')
    .expand('principal')
    .get();

```