---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ae3e3e65f2a60a70dc7de9b6dc66b5713702636
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bookingBusiness = new BookingBusiness
{
    Email = "admin@fabrikam.com",
    SchedulingPolicy = new BookingSchedulingPolicy
    {
        TimeSlotInterval = new Duration("PT60M"),
        MinimumLeadTime = new Duration("P1D"),
        MaximumAdvance = new Duration("P30D"),
        SendConfirmationsToOwner = true,
        AllowStaffSelection = true
    }
};

await graphClient.BookingBusinesses["{bookingBusiness-id}"]
    .Request()
    .UpdateAsync(bookingBusiness);

```