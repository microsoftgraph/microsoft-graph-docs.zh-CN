---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1655d195c8cd551f821802ce79f7620cdb16691930c285b9e9e26f5865dbc900
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const outlookTask = {
  subject: 'Shop for children\'s weekend',
  startDateTime: {
      dateTime: '2016-05-03T09:00:00',
      timeZone: 'Eastern Standard Time'
  },
  dueDateTime: {
      dateTime: '2016-05-05T16:00:00',
      timeZone: 'Eastern Standard Time'
  }
};

await client.api('/me/outlook/tasks')
    .version('beta')
    .post(outlookTask);

```