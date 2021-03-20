---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 939fec6e7684916e37ef9223c407eb9d003633f9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950785"
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