---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b1740617a473ae4afcb2272b3947c87846c04c7
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "42281511"
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
    content: "Does next month work for you?"
  },
  start: {
      dateTime: "2019-03-10T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2019-03-10T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  location:{
      displayName:"Harry's Bar"
  },
  attendees: [
    {
      emailAddress: {
        address:"adelev@contoso.onmicrosoft.com",
        name: "Adele Vance"
      },
      type: "required"
    }
  ],
  transactionId:"7E163156-7762-4BEB-A1C6-729EA81755A7"
};

let res = await client.api('/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events')
    .version('beta')
    .post(event);

```