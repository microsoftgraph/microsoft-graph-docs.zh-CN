---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e081e829195c0bb2ba7cedd7a9373a38c7e07331
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946819"
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
    reviewSettings: {
        isEnabled: true,
        expirationBehavior: 'keepAccess',
        isRecommendationEnabled: true,
        isReviewerJustificationRequired: true,
        isSelfReview: false,
        schedule: {
            startDateTime: '2022-07-02T06:59:59.998Z',
            expiration: {
                duration: 'P14D',
                type: 'afterDuration'
            },
            recurrence: {
                pattern: {
                    type: 'absoluteMonthly',
                    interval: 3,
                    month: 0,
                    dayOfMonth: 0,
                    daysOfWeek: []
                },
                range: {
                    type: 'noEnd',
                    numberOfOccurrences: 0
                }
            }
        },
        primaryReviewers: [
            {
                '@odata.type': '#microsoft.graph.groupMembers',
                groupId: '1623f912-5e86-41c2-af47-39dd67582b66'
            }
        ],
        fallbackReviewers: []
    },
    accessPackage: {
        id: 'a2e1ca1e-4e56-47d2-9daa-e2ba8d12a82b'
    }
};

await client.api('/identityGovernance/entitlementManagement/assignmentPolicies')
    .post(accessPackageAssignmentPolicy);

```