---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d0cf44cc55d98b40dd63a24419fe625f18eddca
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720263"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: "reason-value",
  duration: "duration-value",
  ticketNumber: "ticketNumber-value",
  ticketSystem: "ticketSystem-value"
};

let res = await client.api('/privilegedRoles/{id}/selfActivate')
    .version('beta')
    .post(privilegedRoleAssignment);

```