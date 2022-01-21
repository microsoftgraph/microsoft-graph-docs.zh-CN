---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 081ca2d35abf8a68d06a1e7a1b8f9e0f24ccf964
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129993"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    Email = "admin@fabrikam.com"
    SchedulingPolicy = @{
        TimeSlotInterval = "PT60M"
        MinimumLeadTime = "P1D"
        MaximumAdvance = "P30D"
        SendConfirmationsToOwner = $true
        AllowStaffSelection = $true
    }
}

Update-MgBookingBusiness -BookingBusinessId $bookingBusinessId -BodyParameter $params

```