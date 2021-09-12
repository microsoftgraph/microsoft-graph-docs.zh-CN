---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9af69c6fa36de0dd624d77b293e9d6cc30fa6bb353093ed615e40db8603e8574
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163467"
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