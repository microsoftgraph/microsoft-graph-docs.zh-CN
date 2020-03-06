---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9e878a1f952d5d57961f12f787259bee90c892da
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636846"
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
    .post(event);

```