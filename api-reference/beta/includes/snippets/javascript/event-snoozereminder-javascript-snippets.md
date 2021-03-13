---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b261864db62a37309b209598f6c9cf9ebee01700
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782870"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: '2016-10-19T10:37:00Z',
    timeZone: 'timeZone-value'
  }
};

await client.api('/me/events/{id}/snoozeReminder')
    .version('beta')
    .post(snoozeReminder);

```