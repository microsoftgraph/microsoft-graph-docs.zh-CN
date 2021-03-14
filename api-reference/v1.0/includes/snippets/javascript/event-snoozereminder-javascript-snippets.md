---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 306f2de5489e09614c1a046f3cfbdf63d34e0710
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787175"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: 'dateTime-value',
    timeZone: 'timeZone-value'
  }
};

await client.api('/me/events/{id}/snoozeReminder')
    .post(snoozeReminder);

```