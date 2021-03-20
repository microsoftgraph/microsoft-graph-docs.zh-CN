---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 441b249ce06d62ebe508ce234376df769bb71dfa
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const governanceRoleAssignmentRequest = {
  roleDefinitionId: 'ea48ad5e-e3b0-4d10-af54-39a45bbfe68d',
  resourceId: 'e5e7d29d-5465-45ac-885f-4716a5ee74b5',
  subjectId: '918e54be-12c4-4f4c-a6d3-2ee0e3661c51',
  assignmentState: 'Eligible',
  type: 'AdminAdd',
  reason: 'Assign an eligible role',
  schedule: {
    startDateTime: '2018-05-12T23:37:43.356Z',
    endDateTime: '2018-11-08T23:37:43.356Z',
    type: 'Once'
  }
};

await client.api('/privilegedAccess/azureResources/roleAssignmentRequests')
    .version('beta')
    .post(governanceRoleAssignmentRequest);

```