---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fa39a20516fa0e793d6258d3ff8a5a50d7529046e7ae4c4d44883a6bd212ea1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903174"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
   permissionGrantPolicyIdsAssignedToDefaultUserRole: [
   
   ]
};

await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```