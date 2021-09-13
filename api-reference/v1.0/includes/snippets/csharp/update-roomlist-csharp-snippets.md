---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c6a893709ee1482aad6c9eb407b47787307aabdad28a3c3f22c85f2545ca622e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56904102"
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