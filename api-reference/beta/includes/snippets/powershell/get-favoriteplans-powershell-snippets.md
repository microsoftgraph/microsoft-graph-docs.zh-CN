---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62932f9d8fc1dbf94d415a90971583deb0e521e2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349823"
---
```powershell

Import-Module Microsoft.Graph.Planner

# A UPN can also be used as -UserId.
Get-MgUserPlannerFavoritePlan -UserId $userId

```