---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a96568a4c170200ea30be7c25a76ffd755adcee5
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206794"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentScheduleRequest = {
    action: 'adminAssign',
    justification: 'Assign Groups Admin to IT Helpdesk group',
    roleDefinitionId: 'fdd7a751-b60b-444a-984c-02652fe8fa1c',
    directoryScopeId: '/',
    principalId: '071cc716-8147-4397-a5ba-b2105951cc0b',
    scheduleInfo: {
        startDateTime: '2022-04-10T00:00:00Z',
        expiration: {
            type: 'NoExpiration'
        }
    }
};

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests')
    .post(unifiedRoleAssignmentScheduleRequest);

```