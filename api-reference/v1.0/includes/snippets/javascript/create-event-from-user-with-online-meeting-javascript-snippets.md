---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: afa7ca3f020a1c3147816c346b1df924c5e1cdf1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786606"
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
    content: 'Does noon work for you?'
  },
  start: {
      dateTime: '2017-04-15T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2017-04-15T14:00:00',
      timeZone: 'Pacific Standard Time'
  },
  location: {
      displayName: 'Harry\'s Bar'
  },
  attendees: [
    {
      emailAddress: {
        address: 'samanthab@contoso.onmicrosoft.com',
        name: 'Samantha Booth'
      },
      type: 'required'
    }
  ],
  allowNewTimeProposals: true,
  isOnlineMeeting: true,
  onlineMeetingProvider: 'teamsForBusiness'
};

await client.api('/me/events')
    .post(event);

```