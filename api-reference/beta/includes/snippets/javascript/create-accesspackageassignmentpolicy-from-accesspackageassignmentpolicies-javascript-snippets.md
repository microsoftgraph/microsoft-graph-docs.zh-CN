---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e37bc475cf2a74661619f28ab174d323b24d1544
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807095"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  accessPackageId: '56ff43fd-6b05-48df-9634-956a777fce6d',
  displayName: 'direct',
  description: 'direct assignments by administrator',
  accessReviewSettings: null,
  requestorSettings: {
    scopeType: 'NoSubjects',
    acceptRequests: true,
    allowedRequestors: []
  },
  requestApprovalSettings: {
    isApprovalRequired: false,
    isApprovalRequiredForExtension: false,
    isRequestorJustificationRequired: false,
    approvalMode: 'NoApproval',
    approvalStages: []
  }
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```