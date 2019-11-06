---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f370e2e16ebe1b3050482e2a7f7ee19439079f74
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "38000167"
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
  isReminderOn: true
};

let res = await client.api('/me/events/{id}')
    .version('beta')
    .update(event);

```