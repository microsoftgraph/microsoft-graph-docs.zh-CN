---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac9625b11a2ec2b235ce8ec6af388614507d718e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35493105"
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
    .post({event : event});

```