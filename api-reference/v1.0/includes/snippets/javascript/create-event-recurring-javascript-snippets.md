---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 082be8327f65d0105fae3b7e9c3f997e0871d09c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: 'Let\'s go for lunch',
  body: {
    contentType: 'HTML',
    content: 'Does noon time work for you?'
  },
  start: {
      dateTime: '2017-09-04T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2017-09-04T14:00:00',
      timeZone: 'Pacific Standard Time'
  },
  recurrence: {
    pattern: {
      type: 'weekly',
      interval: 1,
      daysOfWeek: [ 'Monday' ]
    },
    range: {
      type: 'endDate',
      startDate: '2017-09-04',
      endDate: '2017-12-31'
    }
  },
  location: {
      displayName: 'Harry\'s Bar'
  },
  attendees: [
    {
      emailAddress: {
        address: 'AdeleV@contoso.onmicrosoft.com',
        name: 'Adele Vance'
      },
      type: 'required'
    }
  ],
  allowNewTimeProposals: true
};

await client.api('/me/events')
    .post(event);

```