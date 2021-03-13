---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c0070058e69412aa3c03b649830a571f38ca2284
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782037"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  userId: 'userId-value',
  roleId: 'roleId-value'
};

await client.api('/privilegedRoleAssignments')
    .version('beta')
    .post(privilegedRoleAssignment);

```