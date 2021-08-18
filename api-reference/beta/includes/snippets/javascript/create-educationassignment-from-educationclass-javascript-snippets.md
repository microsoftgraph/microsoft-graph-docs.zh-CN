---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d66a4acdb4d7d4b6a8254e26f465ac5a28fcbae8
ms.sourcegitcommit: 22bd45d272681658d46a8b99af3c3eabc7b05cb1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2021
ms.locfileid: "58384378"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
  dueDateTime: '2014-02-01T00:00:00Z',
  displayName: 'Midterm 1',
    instructions: {
      contentType: 'text',
      content: 'Read chapters 1 through 3'
    },
      grading: {
        '@odata.type': '#microsoft.graph.educationAssignmentPointsGradeType',
        maxPoints: 100
      },
      assignTo: {
        '@odata.type': '#microsoft.graph.educationAssignmentClassRecipient'
      },
      status: 'draft',
      allowStudentsToAddResourcesToSubmission: true
};

await client.api('/education/classes/8b8cec7f-d0d8-4974-982a-e29396ddbe7f/assignments')
    .version('beta')
    .post(educationAssignment);

```