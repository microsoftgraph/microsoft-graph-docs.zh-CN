---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1af2bccbdafd80ca5645b4bc1cdb2a0f5a0d4e7
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230733"
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
    content: "Does mid month work for you?"
  },
  start: {
      dateTime: "2019-03-15T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2019-03-15T14:00:00",
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
    .post(event);

```