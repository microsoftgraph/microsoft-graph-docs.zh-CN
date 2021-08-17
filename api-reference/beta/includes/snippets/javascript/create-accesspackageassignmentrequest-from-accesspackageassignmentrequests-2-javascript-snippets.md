---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5464a865fc2330ede37bd328b003ff549ab55815
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
    requestType: 'UserAdd',
    accessPackageAssignment: {
        targetId: '46184453-e63b-4f20-86c2-c557ed5d5df9',
        assignmentPolicyId: '2264bf65-76ba-417b-a27d-54d291f0cbc8',
        accessPackageId: 'a914b616-e04e-476b-aa37-91038f0b165b'
    },
    answers: [
        {
            '@odata.type': '#microsoft.graph.accessPackageAnswerString',
            value: 'Arizona',
            answeredQuestion: {
                '@odata.type': '#microsoft.graph.accessPackageMultipleChoiceQuestion',
                id: 'A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF'
            }
        },
        {
            '@odata.type': '#microsoft.graph.accessPackageAnswerString',
            value: 'Need access to marketing campaign material',
            answeredQuestion: {
                '@odata.type': '#microsoft.graph.accessPackageTextInputQuestion',
                id: 'AA615EE9-D9D8-4C03-BE91-BEE37106DEDA'
            }
        }
    ]
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```