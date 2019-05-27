---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e377a08d5d7b60205e75d095df63e3b71c39f77
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34480853"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: "Plan summer company picnic",
  body: {
    contentType: "HTML",
    content: "Let's kick-start this event planning!"
  },
  start: {
      dateTime: "2017-08-30T11:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2017-08-30T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  attendees: [
    {
      emailAddress: {
        address: "DanaS@contoso.onmicrosoft.com",
        name: "Dana Swope"
      },
      type: "Required"
    },
    {
      emailAddress: {
        address: "AlexW@contoso.onmicrosoft.com",
        name: "Alex Wilber"
      },
      type: "Required"
    }
  ],
  location: {
    displayName: "Conf Room 3; Fourth Coffee; Home Office",
    locationType: "Default"
  },
  locations: [
    {
      displayName: "Conf Room 3"
    },
    {
      displayName: "Fourth Coffee",
      address: {
        street: "4567 Main St",
        city: "Redmond",
        state: "WA",
        countryOrRegion: "US",
        postalCode: "32008"
      },
      coordinates: {
        latitude: 47.672,
        longitude: -102.103
      }
    },
    {
      displayName: "Home Office"
    }
  ]

};

let res = await client.api('/me/events')
    .version('beta')
    .post({event : event});

```