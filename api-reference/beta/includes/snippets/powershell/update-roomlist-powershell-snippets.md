---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6083b917ac7d3a699c60347f8d729a1e57110f8
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62118622"
---
```powershell

Import-Module Microsoft.Graph.Calendar

$params = @{
    "@odata.type" = "microsoft.graph.roomList"
    DisplayName = "Building 1"
    Phone = "555-555-0100"
    Address = @{
        Street = "4567 Main Street"
        City = "Buffalo"
        State = "NY"
        PostalCode = "98052"
        CountryOrRegion = "USA"
    }
    GeoCoordinates = @{
        Altitude = $null
        Latitude = 47
        Longitude = -122
        Accuracy = $null
        AltitudeAccuracy = $null
    }
}

Update-MgPlace -PlaceId $placeId -BodyParameter $params

```