---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 41bea0ae09b8a81a6a5b3ed70095f25486107f3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448444"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  accessPackageId: "56ff43fd-6b05-48df-9634-956a777fce6d",
  displayName: "direct",
  description: "direct assignments by administrator",
  isDenyPolicy: false,
  accessReviewSettings: null,
  requestorSettings: {
    scopeType: "NoSubjects",
    acceptRequests: true,
    allowedRequestors: []
  },
  requestApprovalSettings: {
    isApprovalRequired: false,
    isApprovalRequiredForExtension: false,
    isRequestorJustificationRequired: false,
    approvalMode: "NoApproval",
    approvalStages: []
  }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```