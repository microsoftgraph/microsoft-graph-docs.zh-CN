---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 917eb4efb3a6143b6c7d895d7de6dba27be13c912bca62c4fa56dcd3299137c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54240521"
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