---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 936837c10f2f3b571dccdda3305e2ca5c583ad23
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
    accessPackageId: "string (identifier)",
    displayName: "Users from connected organizations can request",
    description: "Allow users from configured connected organizations to request and be approved by their sponsors",
    canExtend: false,
    durationInDays: 365,
    expirationDateTime: null,
    requestorSettings: {
        scopeType: "AllExistingConnectedOrganizationSubjects",
        acceptRequests: true,
        allowedRequestors: []
    },
    requestApprovalSettings: {
        isApprovalRequired: true,
        isApprovalRequiredForExtension: false,
        isRequestorJustificationRequired: true,
        approvalMode: "Serial",
        approvalStages: [
            {
                approvalStageTimeOutInDays: 14,
                isApproverJustificationRequired: true,
                isEscalationEnabled: true,
                escalationTimeInMinutes: 11520,
                primaryApprovers: [
                    {
                        @odata.type: "#microsoft.graph.groupMembers",
                        isBackup: true,
                        id: "string (identifier)",
                        description: "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        @odata.type: "#microsoft.graph.externalSponsors",
                        isBackup: false
                    }
                ],
                escalationApprovers: [
                    {
                        @odata.type: "#microsoft.graph.singleUser",
                        isBackup: true,
                        id: "string (identifier)",
                        description: "user if the external sponsor does not respond"
                    }
                ]
            },
            {
                approvalStageTimeOutInDays: 14,
                isApproverJustificationRequired: true,
                isEscalationEnabled: true,
                escalationTimeInMinutes: 11520,
                primaryApprovers: [
                    {
                        @odata.type: "#microsoft.graph.groupMembers",
                        isBackup: true,
                        id: "string (identifier)",
                        description: "group for users from connected organizations which have no internal sponsor"
                    },
                    {
                        @odata.type: "#microsoft.graph.internalSponsors",
                        isBackup: false
                    }
                ],
                escalationApprovers: [
                    {
                        @odata.type: "#microsoft.graph.singleUser",
                        isBackup: true,
                        id: "string (identifier)",
                        description: "user if the internal sponsor does not respond"
                    }
                ]
            }
        ]
    },
    accessReviewSettings: {
        isEnabled: true,
        recurrenceType: "quarterly",
        reviewerType: "Self",
        startDateTime: "2020-04-01T07:59:59.998Z",
        durationInDays: 25,
        reviewers: []
    }
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```