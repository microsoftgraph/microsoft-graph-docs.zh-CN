---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26385875e05cad6d7acccdef52d79971f968264c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/oauth2PermissionGrants/{id}')
    .delete();

```