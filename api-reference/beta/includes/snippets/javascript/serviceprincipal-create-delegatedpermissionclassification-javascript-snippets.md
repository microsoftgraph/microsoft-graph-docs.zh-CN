---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8607fdff03e4aaae2ab33f85783833883b592294
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904779"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const delegatedPermissionClassification = {
  permissionId: "e1fe6dd8-ba31-4d61-89e7-88639da4683d",
  permissionName: "User.Read",
  classification: "low"
};

let res = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .post(delegatedPermissionClassification);

```