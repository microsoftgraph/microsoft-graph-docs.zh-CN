---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d87008efe14c7fd525e7fa4730b79549f6a8860b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50950784"
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