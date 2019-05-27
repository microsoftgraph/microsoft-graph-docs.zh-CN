---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f91eaf4712d64c227a89904320fcf15e9d42aa6a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34476575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  originalStartTimeZone: "originalStartTimeZone-value",
  originalEndTimeZone: "originalEndTimeZone-value",
  responseStatus: {
    response: "",
    time: "datetime-value"
  },
  uid: "iCalUId-value",
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

let res = await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==')
    .version('beta')
    .update({conversationThread : conversationThread});

```