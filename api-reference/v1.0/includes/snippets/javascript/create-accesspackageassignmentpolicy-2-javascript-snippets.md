---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d56317847e8586a647ce92d496f1a7de1fe34d6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209626"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
    displayName: 'policy for external access requests',
    description: 'policy for users from connected organizations to request access, with two stages of approval.',
    allowedTargetScope: 'allConfiguredConnectedOrganizationUsers',
    specificAllowedTargets: [],
    expiration: {
        type: 'noExpiration'
    },
    requestorSettings: {
        enableTargetsToSelfAddAccess: true,
        enableTargetsToSelfUpdateAccess: true,
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
                durationBeforeAutomaticDenial: 'P14D',
                isApproverJustificationRequired: false,
                isEscalationEnabled: false,
                durationBeforeEscalation: 'PT0S',
                primaryApprovers: [
                    {
                        '@odata.type': '#microsoft.graph.internalSponsors'
                    }
                ],
                fallbackPrimaryApprovers: [
                    {
                        '@odata.type': '#microsoft.graph.singleUser',
                        userId: '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'
                    },
                    {
                        '@odata.type': '#microsoft.graph.groupMembers',
                        groupId: '1623f912-5e86-41c2-af47-39dd67582b66'
                    }
                ],
                escalationApprovers: [],
                fallbackEscalationApprovers: []
            },
            {
                durationBeforeAutomaticDenial: 'P14D',
                isApproverJustificationRequired: false,
                isEscalationEnabled: false,
                durationBeforeEscalation: 'PT0S',
                primaryApprovers: [],
                fallbackPrimaryApprovers: [
                    {
                        '@odata.type': '#microsoft.graph.singleUser',
                        userId: '46184453-e63b-4f20-86c2-c557ed5d5df9'
                    },
                    {
                        '@odata.type': '#microsoft.graph.groupMembers',
                        groupId: '1623f912-5e86-41c2-af47-39dd67582b66'
                    }
                ],
                escalationApprovers: [],
                fallbackEscalationApprovers: []
            }
        ]
    },
    accessPackage: {
        id: 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'
    }
};

await client.api('/identityGovernance/entitlementManagement/assignmentPolicies')
    .post(accessPackageAssignmentPolicy);

```