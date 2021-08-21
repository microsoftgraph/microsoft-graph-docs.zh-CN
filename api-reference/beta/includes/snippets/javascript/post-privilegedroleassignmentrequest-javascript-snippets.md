---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d15b4a00787a8049a1526ed4c8b661a284e9eeb5213eed2ad99145af1f87f739
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904228"
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