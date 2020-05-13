---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4befcc839024f0275b7a93fdd40b6ef5e32e36c3
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "37994920"
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
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness"
};

let res = await client.api('/me/calendars/AAMkAGViNDU8zAAAAAGtlAAA=/events')
    .version('beta')
    .post(event);

```