---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb4fa7255c0f93be662224c27d5c539a645a5506
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785133"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackage = await client.api('/identityGovernance/entitlementManagement/accessPackages/{id}')
    .version('beta')
    .expand('accessPackageResourceRoleScopes($expand=accessPackageResourceRole,accessPackageResourceScope)')
    .get();

```