---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: befa5116c156b2dac51023b7d9ce83308c625afa00f786e0c26346e37f16f360
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104572"
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
  iCalUId: 'iCalUId-value',
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==')
    .update(conversationThread);

```