---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f370d44af8c1546b6f6432fcc554f05fb00d2d6fb38f102aa71e76488d2f723d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218423"
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
    content: 'Does mid month work for you?'
  },
  start: {
      dateTime: '2019-03-15T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2019-03-15T14:00:00',
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
  transactionId: '7E163156-7762-4BEB-A1C6-729EA81755A7'
};

await client.api('/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events')
    .post(event);

```