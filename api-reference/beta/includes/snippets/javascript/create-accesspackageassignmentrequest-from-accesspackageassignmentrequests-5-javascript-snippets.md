---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2acc31b525381adb4762be90be41d0696d2b89e1
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60355182"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
  requestType: 'AdminAdd',
  accessPackageAssignment: {
     target: {
        email: 'user@contoso.com'
     },
     assignmentPolicyId: '2264bf65-76ba-417b-a27d-54d291f0cbc8',
     accessPackageId: 'a914b616-e04e-476b-aa37-91038f0b165b'
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```