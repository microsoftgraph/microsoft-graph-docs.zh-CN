---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed72a04dbf0d7aca7e16c31f4b4d5bfbd8980d06
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47842839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
    defaultUserRolePermissions:
    {
      allowedToCreateApps: false
    }
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```