---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a1d7956399b669ea5582704d77acdda3d8ef698
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116378"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Get-MgBookingBusinessStaffMember -BookingBusinessId $bookingBusinessId -BookingStaffMemberId $bookingStaffMemberId

```