---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dedf277dc4acf73598a82727933e4c35be1eeb65
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341927"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    ServicePlanId = "28f42d6f-8034-4a0f-9d8a-a218a63b3299"
    SkuId = "465a2a90-5e59-456d-a7b8-127b9fb2e484"
}

# A UPN can also be used as -UserId.
Initialize-MgUserServicePlan -UserId $userId -BodyParameter $params

```