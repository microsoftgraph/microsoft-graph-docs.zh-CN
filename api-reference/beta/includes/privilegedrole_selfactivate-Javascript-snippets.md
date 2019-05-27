---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9d0cf44cc55d98b40dd63a24419fe625f18eddca
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443213"
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