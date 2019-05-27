---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6b16750ee6f6a4539b3c7fadde29a4a4c68edc75
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  assignedTo: "Dana Swope",
  subject: "Shop for children's weekend",
  startDateTime: {
      dateTime: "2016-05-03T09:00:00",
      timeZone: "Eastern Standard Time"
  },
  dueDateTime:  {
      dateTime: "2016-05-05T16:00:00",
      timeZone: "Eastern Standard Time"
  }
};

let res = await client.api('/me/outlook/tasks')
    .version('beta')
    .post({outlookTask : outlookTask});

```