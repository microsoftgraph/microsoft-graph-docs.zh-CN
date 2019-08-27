---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c17de559d813adcff767be789e32b1c1f5e3475b
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636696"
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
    .post(privilegedRoleAssignmentRequest);

```