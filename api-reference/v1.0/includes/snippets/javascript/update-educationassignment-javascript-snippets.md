---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7aea8835a7f79e47a67664851eb1196758553bca
ms.sourcegitcommit: 8ae180a32dbd5a2b12512aee64699a2c23b8678b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2021
ms.locfileid: "60365800"
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
    addedStudentAction: 'none'
};

await client.api('/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignments/4679bc1b-90c5-45af-ae1a-d5357672ed39')
    .update(educationAssignment);

```