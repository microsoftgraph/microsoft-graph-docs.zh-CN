---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d54bf0212456c154d6b2990a8d0ec686422a1969
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333559"
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
    .post(event);

```