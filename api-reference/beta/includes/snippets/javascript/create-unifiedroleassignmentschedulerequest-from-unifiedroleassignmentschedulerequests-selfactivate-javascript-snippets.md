---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3eda9e52a8292496864cb26b1d181b7714aca9f
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentScheduleRequest = {
    action: 'SelfActivate',
    principalId: 'c6ad1942-4afa-47f8-8d48-afb5d8d69d2f',
    roleDefinitionId: '9b895d92-2cd3-44c7-9d02-a6ac2d5ea5c3',
    directoryScopeId: '/',
    justification: 'Need to update app roles for selected apps.',
    scheduleInfo: {
        startDateTime: '2021-08-17T17:40:00.000Z',
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
    .version('beta')
    .post(unifiedRoleAssignmentScheduleRequest);

```