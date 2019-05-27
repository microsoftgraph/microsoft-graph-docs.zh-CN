---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b0bedd6348a4dafd1ab434afa5f4c03de3babff
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460732"
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