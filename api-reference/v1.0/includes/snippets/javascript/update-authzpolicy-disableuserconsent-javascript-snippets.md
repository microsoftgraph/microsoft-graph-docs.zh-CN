---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5dc62eb2a5d0d2064aed7acc61e49b7311960fe4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804066"
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