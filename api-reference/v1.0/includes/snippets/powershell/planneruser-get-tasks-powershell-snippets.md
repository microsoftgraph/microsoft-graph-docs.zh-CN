---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d776c8c8b544fd77600f646ff69b134c8cd3b0ef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352746"
---
```powershell

Import-Module Microsoft.Graph.Planner

# A UPN can also be used as -UserId.
Get-MgUserPlannerTask -UserId $userId

```