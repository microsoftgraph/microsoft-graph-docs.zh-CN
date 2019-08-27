---
description: 自动生成的文件。 不修改
ms.openlocfilehash: deb9513609d85c95e42d11a32ca3d15ea7d61ebb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636718"
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
    .update(oAuth2PermissionGrant);

```