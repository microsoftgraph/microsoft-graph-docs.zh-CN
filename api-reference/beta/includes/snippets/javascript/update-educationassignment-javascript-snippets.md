---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c96625cc31b35d12993605ef07588d51512d0a56
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365838"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
    displayName: 'Reading and review test 09.03 #5',
    instructions: {
        contentType: 'text',
        content: 'Read chapter 5 and write your review'
    },
    dueDateTime: '2021-09-10T00:00:00Z',
    addedStudentAction: 'none',
    addToCalendarAction: 'studentsAndPublisher'
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39')
    .version('beta')
    .update(educationAssignment);

```