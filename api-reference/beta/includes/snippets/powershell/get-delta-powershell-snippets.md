---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 05b96f59142bd469e966f70ad2f74067898d7b25
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347100"
---
```powershell

Import-Module Microsoft.Graph.Users.Functions

# A UPN can also be used as -UserId.
Get-MgUserPlannerAllDelta -UserId $userId

```