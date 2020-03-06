---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c7a1cdbc906daaaaeb95bad21aa56f9961a9c47
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280711"
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
    content: "Does noon work for you?"
  },
  start: {
      dateTime: "2020-02-21T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2020-02-21T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  location:{
      displayName:"Harry's Bar"
  },
  attendees: [
    {
      emailAddress: {
        address:"AlexW@contoso.OnMicrosoft.com",
        name: "Alex Wilbur"
      },
      type: "required"
    }
  ],
  recurrence: {
    pattern: {
      type: "daily",
      interval: 1
    },
    range: {
      type: "numbered",
      startDate: "2020-02-21",
      numberOfOccurrences: 2
    }
  }
};

let res = await client.api('/me/events')
    .post(event);

```