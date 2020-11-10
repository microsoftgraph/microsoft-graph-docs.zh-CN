---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9bdb8dd59c4aa55c489179bbfb4dcbc3b8d617de
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48971687"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.roomList",
  displayName: "Building 1",
  phone:"555-555-0100",
  address: {
    street: "4567 Main Street",
    city: "Buffalo",
    state: "NY",
    postalCode: "98052",
    countryOrRegion: "USA"
  },
  geoCoordinates: {
    altitude: null,
    latitude: 47.0,
    longitude: -122.0,
    accuracy: null,
    altitudeAccuracy: null
 }
};

let res = await client.api('/places/Building1RroomList@contoso.onmicrosoft.com')
    .version('beta')
    .update(place);

```