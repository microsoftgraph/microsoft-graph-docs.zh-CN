---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 04fa3770f079cf47be9abece1396139c0c056175
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var place = new Roomlist
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