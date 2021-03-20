---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e1b70d68cf6ba22788d4f106d5c97f4dbb95e70
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950786"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: '70521f3e-3b95-4e51-b4d2-a2f485b02103',
  resourceId: 'e5e7d29d-5465-45ac-885f-4716a5ee74b5',
  subjectId: '1566d11d-d2b6-444a-a8de-28698682c445',
  assignmentState: 'Eligible',
  type: 'AdminUpdate',
  schedule: {
    type: 'Once',
    startDateTime: '2018-03-08T05:42:45.317Z',
    endDateTime: '2018-06-05T05:42:31.000Z'
  }
};

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```