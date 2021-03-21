---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26aef4173a2504691367a38cdd83a92e6f3e0dce
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973449"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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
geoCoordinates.altitude = 0d;
geoCoordinates.latitude = 47.0d;
geoCoordinates.longitude = -122.0d;
geoCoordinates.accuracy = 0d;
geoCoordinates.altitudeAccuracy = 0d;
place.geoCoordinates = geoCoordinates;

graphClient.places("Building1RroomList@contoso.onmicrosoft.com")
    .buildRequest()
    .patch(place);

```