---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9c78ba233d019164f0297350da21e18371554d0
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46512298"
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
  ],
  allowNewTimeProposals: true
};

let res = await client.api('/me/events')
    .post(event);

```