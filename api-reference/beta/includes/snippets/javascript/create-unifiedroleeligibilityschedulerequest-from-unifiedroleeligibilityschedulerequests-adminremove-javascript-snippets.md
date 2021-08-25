---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 719da09577073fb5012a6b9b3d9e8b66ae27bfbb
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513978"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleEligibilityScheduleRequest = {
    action: 'AdminRemove',
    justification: 'Assign User Admin eligibility to IT Helpdesk (User) group',
    roleDefinitionId: 'fdd7a751-b60b-444a-984c-02652fe8fa1c',
    directoryScopeId: '/',
    principalId: '07706ff1-46c7-4847-ae33-3003830675a1',
    scheduleInfo: {
        startDateTime: '2021-07-26T18:08:06.2081758Z',
        expiration: {
            endDateTime: '2022-06-30T00:00:00Z',
            type: 'AfterDateTime'
        }
    }
};

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .version('beta')
    .post(unifiedRoleEligibilityScheduleRequest);

```