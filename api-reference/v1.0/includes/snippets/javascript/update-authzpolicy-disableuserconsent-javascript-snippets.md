---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 39081420a85d3e3b081db58d210518fdb3690e1095a18ee6abe7bb055df01b3b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277584"
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

await client.api('/policies/authorizationPolicy')
    .update(authorizationPolicy);

```