---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bf6d32df88ed408f70a1849278aed66a8470b94
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691407"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions: {
      permissionGrantPoliciesAssigned: []
   }
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```