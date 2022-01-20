---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1c2f95766f04588810c87767f7d56f04c8f78d37
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62131687"
---
```powershell

Import-Module Microsoft.Graph.Bookings

Remove-MgBookingBusinessStaffMember -BookingBusinessId $bookingBusinessId -BookingStaffMemberId $bookingStaffMemberId

```