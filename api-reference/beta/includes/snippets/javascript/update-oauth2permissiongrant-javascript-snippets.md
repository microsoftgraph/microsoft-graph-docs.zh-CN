---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b0bedd6348a4dafd1ab434afa5f4c03de3babff
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35520119"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  scope: "scope-value"
};

let res = await client.api('/oAuth2Permissiongrants/{id}')
    .version('beta')
    .update({oAuth2PermissionGrant : oAuth2PermissionGrant});

```