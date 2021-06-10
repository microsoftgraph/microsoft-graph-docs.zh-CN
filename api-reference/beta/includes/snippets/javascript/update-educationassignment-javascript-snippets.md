---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e55221445899d81788c9d91e6b7e2900e3ead53
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871504"
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