---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d69fb1bad2e08b473706cd2d6dce062a1696c11280ed696e0f54b5af1356da6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105770"
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