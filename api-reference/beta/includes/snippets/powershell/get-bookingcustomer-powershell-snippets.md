---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aaecaa211725cc11ce2783c2625b0274cbb4ac64
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113956"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Get-MgBookingBusinessCustomer -BookingBusinessId $bookingBusinessId -BookingCustomerId $bookingCustomerId

```