---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a05e5245d17b10b514077b050575cf45755fb428
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2021
ms.locfileid: "52992118"
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
        '@odata.type': 'educationAssignmentPointsGradeType',
        maxPoints: 100
      },
      assignTo: {
        '@odata.type': 'educationAssignmentClassRecipient'
      },
      status: 'draft',
      allowStudentsToAddResourcesToSubmission: true
};

await client.api('/education/classes/8ddcac47-0b45-4cdb-b10a-d36a07a3dd62/assignments')
    .post(educationAssignment);

```