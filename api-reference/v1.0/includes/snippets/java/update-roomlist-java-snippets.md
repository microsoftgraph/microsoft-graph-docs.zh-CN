---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b245971e6136f89890aa873be2b3068575fb9c9
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336380"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Roomlist place = new Roomlist();
place.displayName = "Building 1";
place.phone = "555-555-0100";
PhysicalAddress address = new PhysicalAddress();
address.street = "4567 Main Street";
address.city = "Buffalo";
address.state = "NY";
address.postalCode = "98052";
address.countryOrRegion = "USA";
place.address = address;
OutlookGeoCoordinates geoCoordinates = new OutlookGeoCoordinates();
geoCoordinates.altitude = null;
geoCoordinates.latitude = 47.0;
geoCoordinates.longitude = -122.0;
geoCoordinates.accuracy = null;
geoCoordinates.altitudeAccuracy = null;
place.geoCoordinates = geoCoordinates;

graphClient.places("Building1RroomList@contoso.onmicrosoft.com")
    .buildRequest()
    .patch(place);

```