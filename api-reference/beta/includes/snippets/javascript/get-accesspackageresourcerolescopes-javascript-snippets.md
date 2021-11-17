---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6778fe85878c7928b3e36a9ba7d6d7dcca897be9c1f379be79b74a2120a7bfc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158668"
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