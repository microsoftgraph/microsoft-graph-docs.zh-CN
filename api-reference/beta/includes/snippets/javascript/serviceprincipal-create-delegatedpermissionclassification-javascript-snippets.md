---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0ecbfb845334c6d1e8d0e1e820b97bc4e2dba18
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789800"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const delegatedPermissionClassification = {
  permissionId: 'e1fe6dd8-ba31-4d61-89e7-88639da4683d',
  permissionName: 'User.Read',
  classification: 'low'
};

await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .post(delegatedPermissionClassification);

```