---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f11ece4599821f5c57e05e938f3df1917ba95ff
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343493"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    CancellationMessage = "Your appointment has been successfully cancelled. Please call us again."
}

Stop-MgBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId -BodyParameter $params

```