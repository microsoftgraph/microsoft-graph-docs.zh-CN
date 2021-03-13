---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ca39963d09e3cc808e12063a5485ad5f85ff2a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799431"
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
    content: 'Does next month work for you?'
  },
  start: {
      dateTime: '2019-03-10T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2019-03-10T14:00:00',
      timeZone: 'Pacific Standard Time'
  },
  location: {
      displayName: 'Harry\'s Bar'
  },
  attendees: [
    {
      emailAddress: {
        address: 'adelev@contoso.onmicrosoft.com',
        name: 'Adele Vance'
      },
      type: 'required'
    }
  ],
  isOnlineMeeting: true,
  onlineMeetingProvider: 'teamsForBusiness'
};

await client.api('/me/calendars/AAMkAGViNDU8zAAAAAGtlAAA=/events')
    .version('beta')
    .post(event);

```