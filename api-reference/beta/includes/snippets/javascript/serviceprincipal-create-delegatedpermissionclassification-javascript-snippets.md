---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 756a92394474bf72890017ad2b1ef758047c9418e191df693080fb85a72e5d79
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162735"
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