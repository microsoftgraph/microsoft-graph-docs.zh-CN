---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f15b0013d5c7faf0b44441714bdb482e53af8dae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignmentRequest = {
    duration: '2',
    reason: 'Activate the role for business purpose',
    ticketNumber: '234',
    ticketSystem: 'system',
    schedule: {
        startDateTime: '2018-02-08T02:35:17.903Z'
    },
    type: 'UserAdd',
    assignmentState: 'Active',
    roleId: '88d8e3e3-8f55-4a1e-953a-9b9898b8876b'
};

await client.api('/privilegedRoleAssignmentRequests')
    .version('beta')
    .post(privilegedRoleAssignmentRequest);

```