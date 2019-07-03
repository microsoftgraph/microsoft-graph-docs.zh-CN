---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b68d083d65a6c671407a6e2b63541c56e19c3e0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479145"
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
    .version('beta')
    .post({event : event});

```