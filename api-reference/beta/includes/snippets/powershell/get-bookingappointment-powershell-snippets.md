---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70c28187db2fbf7d83347ed9c4fa850b6c260c5d
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094807"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Get-MgBookingBusinessAppointment -BookingBusinessId $bookingBusinessId -BookingAppointmentId $bookingAppointmentId

```