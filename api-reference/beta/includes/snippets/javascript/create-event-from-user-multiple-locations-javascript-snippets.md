---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a4ab55b8ed8f0e52af19706a9b20f754ee24193e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783024"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: 'Plan summer company picnic',
  body: {
    contentType: 'HTML',
    content: 'Let\'s kick-start this event planning!'
  },
  start: {
      dateTime: '2017-08-30T11:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2017-08-30T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  attendees: [
    {
      emailAddress: {
        address: 'DanaS@contoso.onmicrosoft.com',
        name: 'Dana Swope'
      },
      type: 'Required'
    },
    {
      emailAddress: {
        address: 'AlexW@contoso.onmicrosoft.com',
        name: 'Alex Wilber'
      },
      type: 'Required'
    }
  ],
  location: {
    displayName: 'Conf Room 3; Fourth Coffee; Home Office',
    locationType: 'Default'
  },
  locations: [
    {
      displayName: 'Conf Room 3'
    },
    {
      displayName: 'Fourth Coffee',
      address: {
        street: '4567 Main St',
        city: 'Redmond',
        state: 'WA',
        countryOrRegion: 'US',
        postalCode: '32008'
      },
      coordinates: {
        latitude: 47.672,
        longitude: -102.103
      }
    },
    {
      displayName: 'Home Office'
    }
  ],
  allowNewTimeProposals: true
};

await client.api('/me/events')
    .version('beta')
    .post(event);

```