---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51c1941f9534943d7d2f0d66ab88a166df28863f
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110856"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    SenderShiftId = "SHFT_f7e484ed-fdd6-421c-92d9-0bc9e62e2c29"
    SenderMessage = "Having a family emergency, could you take this shift for me?"
    RecipientUserId = "fe278b61-21ac-4872-8b41-1962bbb98e3c"
}

New-MgTeamScheduleOfferShiftRequest -TeamId $teamId -BodyParameter $params

```