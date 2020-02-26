---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1554605ab5ae37a5fd35949463234eb4600ce36f
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42281519"
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
  ],
  allowNewTimeProposals: true,
  transactionId:"7E163156-7762-4BEB-A1C6-729EA81755A7"
};

let res = await client.api('/me/events')
    .version('beta')
    .post(event);

```