---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2f98908ad18694d4ff68256a602cc8743c67d7f7
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48783369"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   permissionGrantPolicyIdsAssignedToDefaultUserRole:[
   
   ]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```