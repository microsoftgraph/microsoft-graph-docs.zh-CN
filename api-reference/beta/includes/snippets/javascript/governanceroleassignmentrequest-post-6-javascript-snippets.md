---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b2236c203da7b8ac889b3d6dc0fd8380010b514
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: '0e88fd18-50f5-4ee1-9104-01c3ed910065',
  resourceId: 'e5e7d29d-5465-45ac-885f-4716a5ee74b5',
  subjectId: '74765671-9ca4-40d7-9e36-2f4a570608a6',
  assignmentState: 'Eligible',
  type: 'AdminExtend',
  reason: 'extend role assignment',
  schedule: {
    type: 'Once',
    startDateTime: '2018-05-12T23:53:55.327Z',
    endDateTime: '2018-08-10T23:53:55.327Z'
  }
};

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```