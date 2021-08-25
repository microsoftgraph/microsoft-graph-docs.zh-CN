---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 73999f944afbb87ce48deacc6a659b3422a4f173
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleAssignmentScheduleRequest = {
  action: 'AdminAssign',
  justification: 'Assign User Admin to IT Helpdesk (User) group',
  roleDefinitionId: 'fdd7a751-b60b-444a-984c-02652fe8fa1c',
  directoryScopeId: '/',
  principalId: '07706ff1-46c7-4847-ae33-3003830675a1',
  scheduleInfo: {
    startDateTime: '2021-07-01T00:00:00Z',
    expiration: {
      type: 'NoExpiration'
    }
  }
};

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/')
    .version('beta')
    .post(unifiedRoleAssignmentScheduleRequest);

```