---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bbfbee4d483a842732ca505f7a6d6c7a3da5ce55
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209604"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  displayName: 'New Policy',
  description: 'policy for assignment',
  allowedTargetScope: 'notSpecified',
  specificAllowedTargets: [],
  expiration: {
      endDateTime: null,
      duration: null,
      type: 'noExpiration'
  },
  requestorSettings: {
      enableTargetsToSelfAddAccess: false,
      enableTargetsToSelfUpdateAccess: false,
      enableTargetsToSelfRemoveAccess: false,
      allowCustomAssignmentSchedule: true,
      enableOnBehalfRequestorsToAddAccess: false,
      enableOnBehalfRequestorsToUpdateAccess: false,
      enableOnBehalfRequestorsToRemoveAccess: false,
      onBehalfRequestors: []
  },
  requestApprovalSettings: {
      isApprovalRequiredForAdd: false,
      isApprovalRequiredForUpdate: false,
      stages: []
  },
  accessPackage: {
      id: 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'
  }
};

await client.api('/identityGovernance/entitlementManagement/assignmentPolicies')
    .post(accessPackageAssignmentPolicy);

```