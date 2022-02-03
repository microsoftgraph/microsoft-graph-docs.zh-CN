---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 33d4d1cdf8335e08cb4068f67eedaed82a874ebf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351655"
---
```powershell

Import-Module Microsoft.Graph.Planner

# A UPN can also be used as -UserId.
Get-MgUserPlannerPlan -UserId $userId

```