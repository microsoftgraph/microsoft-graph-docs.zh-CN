---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd3d1e22c51bb3b35f14b64f1ac6e38ce06b3ad4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636502"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: "0e88fd18-50f5-4ee1-9104-01c3ed910065",
  resourceId: "e5e7d29d-5465-45ac-885f-4716a5ee74b5",
  subjectId: "74765671-9ca4-40d7-9e36-2f4a570608a6",
  assignmentState: "Eligible",
  type: "AdminExtend",
  reason: "extend role assignment",
  schedule: {
    type: "Once",
    startDateTime: "2018-05-12T23:53:55.327Z",
    endDateTime: "2018-08-10T23:53:55.327Z"
  }
};

let res = await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```