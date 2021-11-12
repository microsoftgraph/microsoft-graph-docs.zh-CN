---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5874f6ddfbb157307318879926cf6d4a28e195518a2eee46af6f6535b0e76b5a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333604"
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
  transactionId: '7E163156-7762-4BEB-A1C6-729EA81755A7'
};

await client.api('/me/events')
    .version('beta')
    .post(event);

```