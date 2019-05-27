---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 19409310cc3b55809494bf311405f5e34df8d7d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480881"
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
  ]
};

let res = await client.api('/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events')
    .version('beta')
    .post({event : event});

```