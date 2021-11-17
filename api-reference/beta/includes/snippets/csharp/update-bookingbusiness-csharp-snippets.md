---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4ec9552ddc34346d9e857932c7b2062d5333dd4345294cb45fee3c98d2e4643
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903130"
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