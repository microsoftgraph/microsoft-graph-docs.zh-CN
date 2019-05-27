---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 13e68b69cb420ad9c1e1b9fa8926661e41a4f4f5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436598"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: "2016-10-19T10:37:00Z",
    timeZone: "timeZone-value"
  }
};

let res = await client.api('/me/events/{id}/snoozeReminder')
    .version('beta')
    .post(snoozeReminder);

```