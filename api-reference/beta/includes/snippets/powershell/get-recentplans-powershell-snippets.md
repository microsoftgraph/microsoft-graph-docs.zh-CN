---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53ea60e24e7077c6d2d102ccfdf7a668636b7227
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352106"
---
```powershell

Import-Module Microsoft.Graph.Planner

# A UPN can also be used as -UserId.
Get-MgUserPlannerRecentPlan -UserId $userId

```