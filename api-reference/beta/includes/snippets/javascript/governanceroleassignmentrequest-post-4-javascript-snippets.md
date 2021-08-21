---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e79e75efd30c2b8d84e7dd411879d78019c07fcd14cb37c87e2c67dd08959737
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: '65bb4622-61f5-4f25-9d75-d0e20cf92019',
  resourceId: 'e5e7d29d-5465-45ac-885f-4716a5ee74b5',
  subjectId: '74765671-9ca4-40d7-9e36-2f4a570608a6',
  assignmentState: 'Eligible',
  type: 'AdminRemove'
};

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```