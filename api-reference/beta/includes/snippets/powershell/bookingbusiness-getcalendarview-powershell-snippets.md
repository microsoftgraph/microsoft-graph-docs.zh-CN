---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66841182e85756efa57518954214a0e651808079
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114103"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Get-MgBookingBusinessCalendarView -BookingBusinessId $bookingBusinessId -Start "2018-04-30T00:00:00Z" -End "2018-05-10T00:00:00Z" 

```