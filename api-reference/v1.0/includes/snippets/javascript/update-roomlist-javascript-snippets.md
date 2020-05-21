---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b9a30ac0af28570a14a350404aa962407bf91a25
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336385"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const place = {
  @odata.type: "microsoft.graph.roomlist",
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
    .update(place);

```