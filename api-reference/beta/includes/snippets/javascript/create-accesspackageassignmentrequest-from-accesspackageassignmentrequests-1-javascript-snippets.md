---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef0b0acae309ce27e52a5eac0376ce61310d1b24
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
  requestType: 'AdminAdd',
  accessPackageAssignment: {
     targetId: '46184453-e63b-4f20-86c2-c557ed5d5df9',
     assignmentPolicyId: '2264bf65-76ba-417b-a27d-54d291f0cbc8',
     accessPackageId: 'a914b616-e04e-476b-aa37-91038f0b165b'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```