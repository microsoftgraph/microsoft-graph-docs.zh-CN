---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5cb35e32dc2a2e8e010519790deb677b8b0151211dfd479f214930a538c4bba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104195"
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