---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d205496cccb064ea1be9000866e64c674bf8be32
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignmentRequest = {
    duration: "2",
    reason: "Activate the role for business purpose",
    ticketNumber: "234",
    ticketSystem: "system",
    schedule: {
        startDateTime: "2018-02-08T02:35:17.903Z"
    },
    evaluateOnly: false,
    type: "UserAdd",
    assignmentState: "Active",
    roleId: "88d8e3e3-8f55-4a1e-953a-9b9898b8876b"
};

let res = await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .post({privilegedRoleAssignmentRequest : privilegedRoleAssignmentRequest});

```