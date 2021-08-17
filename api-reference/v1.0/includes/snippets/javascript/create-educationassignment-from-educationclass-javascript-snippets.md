---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ec4ec587b7f7807667a22f28b61bee84c7a49797c652eb74fc873c22bf56373
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57221426"
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