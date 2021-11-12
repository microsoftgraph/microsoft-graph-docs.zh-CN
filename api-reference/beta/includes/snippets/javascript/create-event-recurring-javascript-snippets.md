---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 684199e54611622e0fbe9c15e9fee69fbdfa61c5ed0865ab2a0e9de5dc3c8851
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378354"
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