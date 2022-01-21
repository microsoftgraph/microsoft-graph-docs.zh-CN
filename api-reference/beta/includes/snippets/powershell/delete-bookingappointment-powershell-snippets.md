---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 382ac235cc558577135530abe88435dfe4ee9fd6
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116560"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Remove-MgBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId

```