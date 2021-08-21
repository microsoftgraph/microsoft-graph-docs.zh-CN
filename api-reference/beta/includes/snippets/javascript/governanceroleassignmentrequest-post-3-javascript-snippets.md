---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: beb11bc377eb16d1194798a135f53bd48e1466e46975c5db61c9547bda1ea258
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: 'bc75b4e6-7403-4243-bf2f-d1f6990be122',
  resourceId: 'fb016e3a-c3ed-4d9d-96b6-a54cd4f0b735',
  subjectId: '918e54be-12c4-4f4c-a6d3-2ee0e3661c51',
  assignmentState: 'Active',
  type: 'UserRemove',
  reason: 'Deactivate the role',
  linkedEligibleRoleAssignmentId: 'cb8a533e-02d5-42ad-8499-916b1e4822ec'
};

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```