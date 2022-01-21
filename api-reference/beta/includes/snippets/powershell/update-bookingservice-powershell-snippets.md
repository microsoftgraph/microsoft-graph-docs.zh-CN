---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 929d8e2e092a17e0bda06b050200e755689a2959
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094491"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingService"
    DefaultDuration = "PT30M"
}

Update-MgBookingBusinessService -BookingBusinessId $bookingBusinessId -BookingServiceId $bookingServiceId -BodyParameter $params

```