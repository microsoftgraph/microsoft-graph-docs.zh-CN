---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8a186a8d3a86f1011d3ef8a541feb129e593a562
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
    dueDateTime: '2021-09-07T00:00:00Z',
    displayName: 'Reading test 09.03 #4',
    instructions: {
        contentType: 'text',
        content: 'Read chapter 4'
    },
    grading: {
        '@odata.type': '#microsoft.graph.educationAssignmentPointsGradeType',
        maxPoints: 50
    },
    assignTo: {
        '@odata.type': '#microsoft.graph.educationAssignmentClassRecipient'
    },
    status: 'draft',
    allowStudentsToAddResourcesToSubmission: true
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments')
    .version('beta')
    .post(educationAssignment);

```