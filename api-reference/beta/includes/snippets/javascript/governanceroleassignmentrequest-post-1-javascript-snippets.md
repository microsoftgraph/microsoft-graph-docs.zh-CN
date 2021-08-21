---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbc0bba293eac794095740f1523abb6ec2b8441ff9e690e9a85ecdc3d4f8e29a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105766"
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