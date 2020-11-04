---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d05eea2669d1e3f7217797fd4fb178d7a790562
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904535"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = new RoomList
{
    DisplayName = "Building 1",
    Phone = "555-555-0100",
    Address = new PhysicalAddress
    {
        Street = "4567 Main Street",
        City = "Buffalo",
        State = "NY",
        PostalCode = "98052",
        CountryOrRegion = "USA"
    },
    GeoCoordinates = new OutlookGeoCoordinates
    {
        Altitude = null,
        Latitude = 47,
        Longitude = -122,
        Accuracy = null,
        AltitudeAccuracy = null
    }
};

await graphClient.Places["Building1RroomList@contoso.onmicrosoft.com"]
    .Request()
    .UpdateAsync(place);

```