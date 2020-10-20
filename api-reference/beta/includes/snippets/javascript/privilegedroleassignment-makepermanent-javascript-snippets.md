---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a113ed8c7b0d5a1e519b1b44e1b573d39c9741f5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612434"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: "reason-value",
  ticketNumber: "ticketNumber-value",
  ticketSystem: "ticketSystem-value"
};

let res = await client.api('/privilegedRoleAssignments/{id}/makePermanent')
    .version('beta')
    .post(privilegedRoleAssignment);

```