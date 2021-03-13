---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1bd2f913a7b6237962bea228fd6b55220bcbb1f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809198"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackage = {
  displayName: 'Access Package New Name'
};

await client.api('/identityGovernance/entitlementManagement/accessPackages/{accessPackageId}')
    .version('beta')
    .update(accessPackage);

```