---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb2d98c98fb82ca5e7bacb670b7e363661222cde
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778418"
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
  ]
};

await client.api('/me/events')
    .version('beta')
    .post(event);

```