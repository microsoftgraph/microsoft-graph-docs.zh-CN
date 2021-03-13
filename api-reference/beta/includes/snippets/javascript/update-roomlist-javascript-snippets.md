---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c6e7ac23fbd8a8f851201285076a630c09280f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807891"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  '@odata.type': 'microsoft.graph.roomList',
  displayName: 'Building 1',
  phone: '555-555-0100',
  address: {
    street: '4567 Main Street',
    city: 'Buffalo',
    state: 'NY',
    postalCode: '98052',
    countryOrRegion: 'USA'
  },
  geoCoordinates: {
    altitude: null,
    latitude: 47.0,
    longitude: -122.0,
    accuracy: null,
    altitudeAccuracy: null
 }
};

await client.api('/places/Building1RroomList@contoso.onmicrosoft.com')
    .version('beta')
    .update(place);

```