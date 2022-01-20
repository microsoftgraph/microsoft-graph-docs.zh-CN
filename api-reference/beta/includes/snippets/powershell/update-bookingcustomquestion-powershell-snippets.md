---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0a3379a132e5d758b941aaf7612bcc1aae6e08f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094534"
---
```powershell

Import-Module Microsoft.Graph.Bookings

$params = @{
    "@odata.type" = "#microsoft.graph.bookingCustomQuestion"
    DisplayName = "What is your age?"
    AnswerInputType = "text"
    AnswerOptions = @(
    )
}

Update-MgBookingBusinessCustomQuestion -BookingBusinessId $bookingBusinessId -BookingCustomQuestionId $bookingCustomQuestionId -BodyParameter $params

```