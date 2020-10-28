---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 47c9314daeac8aa264ad7cfbfa75e80de644f5c8
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   permissionGrantPolicyIdsAssignedToDefaultUserRole:[
      "managePermissionGrantsForSelf.microsoft-user-default-low"
   ]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```