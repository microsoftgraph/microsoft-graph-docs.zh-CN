---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf01d8da45a264c6368779ada04e31df2872efa7
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39636963"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: "Prep for customer meeting",
  body: {
    contentType: "HTML",
    content: "Does this time work for you?"
  },
  start: {
      dateTime: "2019-11-20T13:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2019-11-20T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  location:{
      displayName:"Cordova conference room"
  },
  attendees: [
    {
      emailAddress: {
        address:"AdeleV@contoso.OnMicrosoft.com",
        name: "Adele Vance"
      },
      type: "required"
    }
  ],
  allowNewTimeProposals: true,
  isOnlineMeeting: true,
  onlineMeetingProvider: "teamsForBusiness"
};

let res = await client.api('/me/events')
    .version('beta')
    .post(event);

```