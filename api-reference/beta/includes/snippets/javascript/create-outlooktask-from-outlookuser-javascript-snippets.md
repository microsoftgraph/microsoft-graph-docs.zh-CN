---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 7b01cbb78820796b086f8ac715fd38f90b7e33bf
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636710"
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
    .post(outlookTask);

```