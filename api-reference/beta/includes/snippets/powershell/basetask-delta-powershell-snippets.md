---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d314465619efa6afaa6318d51fb5eaf05e7f6b73
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341784"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserTaskListTaskDelta -UserId $userId -BaseTaskListId $baseTaskListId

```