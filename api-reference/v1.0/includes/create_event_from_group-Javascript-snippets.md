---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e3950f95e06175cb69f8c2a2b8bce45a2802ec9
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536251"
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
    content: "Does late morning work for you?"
  },
  start: {
      dateTime: "2019-06-16T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2019-06-16T14:00:00",
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

let res = await client.api('/groups/01d4ee64-15ce-491e-bad1-b91aa3223df4/events')
    .post({event : event});

```