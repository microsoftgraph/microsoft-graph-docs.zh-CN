---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e6120257566d9c5e5e75716822c683916a71a28fa65774ba2bab4aa8a2fb423
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106887"
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