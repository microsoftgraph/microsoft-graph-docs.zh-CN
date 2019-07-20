---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fed23eeec26d1d4d3adcd45dbe0f619bcd0f8f27
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723279"
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
      dateTime: "2017-04-15T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2017-04-15T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  location:{
      displayName:"Harry's Bar"
  },
  attendees: [
    {
      emailAddress: {
        address:"samanthab@contoso.onmicrosoft.com",
        name: "Samantha Booth"
      },
      type: "required"
    }
  ]
};

let res = await client.api('/me/events')
    .post({event : event});

```