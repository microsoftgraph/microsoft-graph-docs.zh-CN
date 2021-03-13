---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5fae20435028c95ac7469e992d681017bccf03a7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796407"
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

await graphClient.Places["{place-id}"]
    .Request()
    .UpdateAsync(place);

```