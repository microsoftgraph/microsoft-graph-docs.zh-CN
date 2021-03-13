---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c69a7cc0f6b88a253408dda0e8ee7763582e73eb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796050"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentMultiple = {
    principalIds: ['0aeec2c1-fee7-4e02-b534-6f920d25b300', '2d5386a7-732f-44db-9cf8-f82dd2a1c0e0']
};

await client.api('/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1')
    .version('beta')
    .update(unifiedRoleAssignmentMultiple);

```