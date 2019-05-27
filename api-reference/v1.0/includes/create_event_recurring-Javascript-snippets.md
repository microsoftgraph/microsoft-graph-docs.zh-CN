---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 91bfa373abf8a46f2793e5fcbbfdfa41bfe5469e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: "Let's go for lunch",
  body: {
    contentType: "HTML",
    content: "Does noon time work for you?"
  },
  start: {
      dateTime: "2017-09-04T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2017-09-04T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  recurrence: {
    pattern: {
      type: "weekly",
      interval: 1,
      daysOfWeek: [ "Monday" ]
    },
    range: {
      type: "endDate",
      startDate: "2017-09-04",
      endDate: "2017-12-31"
    }
  },
  location:{
      displayName:"Harry's Bar"
  },
  attendees: [
    {
      emailAddress: {
        address:"AdeleV@contoso.onmicrosoft.com",
        name: "Adele Vance"
      },
      type: "required"
    }
  ]
};

let res = await client.api('/me/events')
    .post({event : event});

```