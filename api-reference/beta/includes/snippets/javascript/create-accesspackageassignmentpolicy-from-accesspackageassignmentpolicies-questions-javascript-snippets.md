---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b186967683277854f9492a95f851aa440172fb27
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
    accessPackageId: "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
    displayName: "Users from connected organizations can request",
    description: "Allow users from configured connected organizations to request and be approved by their sponsors",
    canExtend: false,
    durationInDays: 365,
    expirationDateTime: null,
    requestorSettings: {
        scopeType: "AllExistingConnectedOrganizationSubjects",
        acceptRequests: true
    },
    requestApprovalSettings: {
        isApprovalRequired: true,
        isApprovalRequiredForExtension: false,
        isRequestorJustificationRequired: true,
        approvalMode: "SingleStage",
        approvalStages: [{
                approvalStageTimeOutInDays: 14,
                isApproverJustificationRequired: true,
                isEscalationEnabled: true,
                escalationTimeInMinutes: 11520,
                primaryApprovers: [{
                        @odata.type: "#microsoft.graph.groupMembers",
                        isBackup: true,
                        id: "d2dcb9a1-a445-42ee-83a8-476522ed6cbf",
                        description: "group for users from connected organizations which have no external sponsor"
                    },
                    {
                        @odata.type: "#microsoft.graph.externalSponsors",
                        isBackup: false
                    }
                ]
            }
        ]
    },
    accessReviewSettings: {
        isEnabled: false
    },
    questions: [{
        isRequired: false,
        text: {
            defaultText: "what state are you from?",
            localizedTexts: [{
                text: "¿De qué estado eres?",
                languageCode: "es"
            }]
        },
        @odata.type: "#microsoft.graph.accessPackageMultipleChoiceQuestion",
        choices: [{
            actualValue: "AZ",
            displayValue: {
                localizedTexts: [{
                    text: "Arizona",
                    languageCode: "es"
                }]
            }
        }, {
            actualValue: "CA",
            displayValue: {
                localizedTexts: [{
                    text: "California",
                    languageCode: "es"
                }]
            }
        }, {
            actualValue: "OH",
            displayValue: {
                localizedTexts: [{
                    text: "Ohio",
                    languageCode: "es"
                }]
            }
        }],
        allowsMultipleSelection: false
    }, {
        isRequired: false,
        text: {
            defaultText: "Who is your manager?",
            localizedTexts: [{
                text: "por qué necesita acceso a este paquete",
                languageCode: "es"
            }]
        },
        @odata.type: "#microsoft.graph.accessPackageTextInputQuestion",
        isSingleLineQuestion: false
    }]
};

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies')
    .version('beta')
    .post(accessPackageAssignmentPolicy);

```