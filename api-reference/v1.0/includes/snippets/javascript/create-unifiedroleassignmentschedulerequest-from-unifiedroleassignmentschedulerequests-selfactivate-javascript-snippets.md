---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 60ca038a149e7294ff21fed1a0f99b20805655ea
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206766"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentScheduleRequest = {
    action: 'selfActivate',
    principalId: '071cc716-8147-4397-a5ba-b2105951cc0b',
    roleDefinitionId: '8424c6f0-a189-499e-bbd0-26c1753c96d4',
    directoryScopeId: '/',
    justification: 'I need access to the Attribute Administrator role to manage attributes to be assigned to restricted AUs',
    scheduleInfo: {
        startDateTime: '2022-04-14T00:00:00.000Z',
        expiration: {
            type: 'AfterDuration',
            duration: 'PT5H'
        }
    },
    ticketInfo: {
        ticketNumber: 'CONTOSO:Normal-67890',
        ticketSystem: 'MS Project'
    }
};

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/')
    .post(unifiedRoleAssignmentScheduleRequest);

```