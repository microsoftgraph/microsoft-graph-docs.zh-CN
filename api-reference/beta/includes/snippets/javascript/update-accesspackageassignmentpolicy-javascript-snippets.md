---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89d27f5eb421f176553561d2321a5e739cd7f6ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentPolicy = {
    id: 'b2eba9a1-b357-42ee-83a8-336522ed6cbf',
    accessPackageId: '4c02f928-7752-49aa-8fc8-e286d973a965',
    displayName: 'All Users',
    description: 'All users can request for access to the directory.',
    canExtend: false,
    durationInDays: 365,
    expirationDateTime: null,
    requestorSettings: {
        scopeType: 'AllExistingConnectedOrganizationSubjects',
        acceptRequests: true,
        allowedRequestors: []
    },
    requestApprovalSettings: {
        isApprovalRequired: true,
        isApprovalRequiredForExtension: false,
        isRequestorJustificationRequired: true,
        approvalMode: 'SingleStage',
        approvalStages: [{
                approvalStageTimeOutInDays: 14,
                isApproverJustificationRequired: true,
                isEscalationEnabled: true,
                escalationTimeInMinutes: 11520,
                primaryApprovers: [{
                        '@odata.type': '#microsoft.graph.groupMembers',
                        isBackup: true,
                        id: 'd2dcb9a1-a445-42ee-83a8-476522ed6cbf',
                        description: 'group for users from connected organizations which have no external sponsor'
                    },
                    {
                        '@odata.type': '#microsoft.graph.externalSponsors',
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
            defaultText: 'what state are you from?',
            localizedTexts: [{
                text: '¿De qué estado eres?',
                languageCode: 'es'
            }]
        },
        '@odata.type': '#microsoft.graph.accessPackageMultipleChoiceQuestion',
        choices: [{
            actualValue: 'AZ',
            displayValue: {
                localizedTexts: [{
                    text: 'Arizona',
                    languageCode: 'es'
                }]
            }
        }, {
            actualValue: 'CA',
            displayValue: {
                localizedTexts: [{
                    text: 'California',
                    languageCode: 'es'
                }]
            }
        }],
        allowsMultipleSelection: false
    }, {
        isRequired: false,
        text: {
            defaultText: 'Who is your manager?',
            localizedTexts: [{
                text: 'por qué necesita acceso a este paquete',
                languageCode: 'es'
            }]
        },
        '@odata.type': '#microsoft.graph.accessPackageTextInputQuestion',
        isSingleLineQuestion: false
    }]
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf')
    .version('beta')
    .put(accessPackageAssignmentPolicy);

```