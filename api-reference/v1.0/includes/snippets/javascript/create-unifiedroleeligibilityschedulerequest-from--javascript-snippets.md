---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d05eb701803cd855950e56799691a1ad9b691a0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65206686"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleEligibilityScheduleRequest = {
    action: 'adminAssign',
    justification: 'Assign Attribute Assignment Admin eligibility to restricted user',
    roleDefinitionId: '8424c6f0-a189-499e-bbd0-26c1753c96d4',
    directoryScopeId: '/',
    principalId: '071cc716-8147-4397-a5ba-b2105951cc0b',
    scheduleInfo: {
        startDateTime: '2022-04-10T00:00:00Z',
        expiration: {
            type: 'afterDateTime',
            endDateTime: '2024-04-10T00:00:00Z'
        }
    }
};

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .post(unifiedRoleEligibilityScheduleRequest);

```