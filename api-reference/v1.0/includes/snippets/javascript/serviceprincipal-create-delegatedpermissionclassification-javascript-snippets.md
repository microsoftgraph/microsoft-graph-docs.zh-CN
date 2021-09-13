---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 092d4c801fa7a02e4ebe9162a7ad8a2e348f4b6e991f9037c2939d4b7294f44f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162349"
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
    .post(delegatedPermissionClassification);

```