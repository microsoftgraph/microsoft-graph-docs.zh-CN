---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46c3f8b319f751b9405954cdcc1da7ed4456c574
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798347"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  scope: 'scope-value'
};

await client.api('/oauth2PermissionGrants/{id}')
    .update(oAuth2PermissionGrant);

```