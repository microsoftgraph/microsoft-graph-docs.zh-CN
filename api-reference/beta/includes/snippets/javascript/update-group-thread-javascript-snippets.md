---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6a76d235f048b258d4f9e74f0270812fb7618c8a0c02c81afac6336a1e24843e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  originalStartTimeZone: 'originalStartTimeZone-value',
  originalEndTimeZone: 'originalEndTimeZone-value',
  responseStatus: {
    response: '',
    time: 'datetime-value'
  },
  uid: 'iCalUId-value',
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==')
    .version('beta')
    .update(conversationThread);

```