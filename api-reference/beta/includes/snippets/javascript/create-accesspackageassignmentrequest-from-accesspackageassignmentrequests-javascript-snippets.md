---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 538feb3bce39291f663a693b370d0603b86c08c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803242"
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
    answers: [{
        '@odata.type': '#microsoft.graph.accessPackageAnswerString',
        value: 'Arizona',
        answeredQuestion: {
            id: 'A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF'
        }
    }, {
        '@odata.type': '#microsoft.graph.accessPackageAnswerString',
        value: 'Need access to marketing campaign material',
        answeredQuestion: {
            id: 'AA615EE9-D9D8-4C03-BE91-BEE37106DEDA'
        }
    }]
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .post(accessPackageAssignmentRequest);

```