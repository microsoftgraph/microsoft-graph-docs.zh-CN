---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d2522b6b8dc677638c7fc07ab525874c40e988b
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   defaultUserRolePermissions:{
      allowedToCreateApps:false
   }
};

let res = await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```