---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5417ce600fb7452203b4b2a2499eb096cc5ad62a
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  originalStartTimeZone: "originalStartTimeZone-value",
  originalEndTimeZone: "originalEndTimeZone-value",
  responseStatus: {
    response: "",
    time: "2016-10-19T10:37:00Z"
  },
  recurrence: null,
  uid: "iCalUId-value",
  reminderMinutesBeforeStart: 99,
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness",
  isReminderOn: true,
  categories: ["Red category"]
};

let res = await client.api('/me/events/{id}')
    .version('beta')
    .update(event);

```