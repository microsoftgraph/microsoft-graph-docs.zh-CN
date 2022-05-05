---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d3f9625388fc055c226c367c3d65119fea88bd83
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
  id: '87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187',
  displayName: 'All Users',
  description: 'All users can request for access to the directory.',
  allowedTargetScope: 'allDirectoryUsers',
  specificAllowedTargets: [],
  expiration: {
      type: 'noExpiration'
  },
  requestorSettings: {
      enableTargetsToSelfAddAccess: true,
      enableTargetsToSelfUpdateAccess: false,
      enableTargetsToSelfRemoveAccess: true,
      allowCustomAssignmentSchedule: false,
      enableOnBehalfRequestorsToAddAccess: false,
      enableOnBehalfRequestorsToUpdateAccess: false,
      enableOnBehalfRequestorsToRemoveAccess: false,
      onBehalfRequestors: []
  },
  requestApprovalSettings: {
      isApprovalRequiredForAdd: true,
      isApprovalRequiredForUpdate: false,
      stages: [
          {
              durationBeforeAutomaticDenial: 'P2D',
              isApproverJustificationRequired: false,
              isEscalationEnabled: false,
              durationBeforeEscalation: 'PT0S',
              primaryApprovers: [
                  {
                      '@odata.type': '#microsoft.graph.requestorManager',
                      managerLevel: 1
                  }
              ],
              fallbackPrimaryApprovers: [
                  {
                      '@odata.type': '#microsoft.graph.singleUser',
                      userId: 'e6bf4d7d-6824-4dd0-809d-5bf42d4817c2',
                      description: 'user'
                  }
              ],
              escalationApprovers: [],
              fallbackEscalationApprovers: []
          }
      ]
  },
  accessPackage: {
        id: '49d2c59b-0a81-463d-a8ec-ddad3935d8a0'
  }
};

await client.api('/identityGovernance/entitlementManagement/assignmentPolicies/87e1c7f7-c7f7-87e1-f7c7-e187f7c7e187')
    .put(accessPackageAssignmentPolicy);

```