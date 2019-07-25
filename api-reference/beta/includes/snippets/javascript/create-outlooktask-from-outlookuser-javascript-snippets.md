---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 849bb3f60f67d9cc44dd65b47faf5b69dac857ff
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35877308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
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