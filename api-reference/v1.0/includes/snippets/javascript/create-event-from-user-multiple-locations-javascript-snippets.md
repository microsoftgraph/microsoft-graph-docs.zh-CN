---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0e667a102221e1d4105955a72a7b31ad85c554cc055143315811a380fcf4fd6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218656"
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
    .post(event);

```