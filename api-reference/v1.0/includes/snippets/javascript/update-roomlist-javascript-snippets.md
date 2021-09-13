---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8609b8bbab6b29a8f47fdf3400b475eb5c9996a75d5d44ac71de8ba84542383d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106776"
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
    .update(place);

```