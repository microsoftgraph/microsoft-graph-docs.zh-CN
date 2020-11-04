---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e1c97953c6272863535cb5d634fb881c56fbbf95
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904533"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RoomList place = new RoomList();
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