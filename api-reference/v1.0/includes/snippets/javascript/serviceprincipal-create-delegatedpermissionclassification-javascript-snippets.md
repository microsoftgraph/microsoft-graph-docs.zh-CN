---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b8ef4d8dba0fafe8435f37c53bbb7d410bbc7fb
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523093"
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
    .post(delegatedPermissionClassification);

```