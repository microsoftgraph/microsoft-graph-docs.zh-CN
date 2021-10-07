---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4aa757a676c5e86a78c1553648bae7ee17a0074afef81ca0ec54a7e87b26ec66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161561"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const educationAssignment = {
  displayName: 'Week 1 reading assignment',
  instructions: {
    contentType: 'Text',
    content: 'Read chapters 1 through 3'
  },
  dueDateTime: '2014-02-01T00:00:00Z',
  addedStudentAction: 'none',
  addToCalendarAction: 'studentsAndPublisher',
};

await client.api('/education/classes/11021/assignments/19002')
    .version('beta')
    .update(educationAssignment);

```