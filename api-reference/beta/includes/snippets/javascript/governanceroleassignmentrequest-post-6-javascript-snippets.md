---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 48a4561466aab8af218e36180b98bdd92fc8801781fd9e80243c44e3d5d100cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105771"
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