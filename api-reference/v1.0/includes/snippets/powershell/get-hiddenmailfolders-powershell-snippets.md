---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 385771c515d86f15f1ddc3900961b209ee67fc49
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351175"
---
```powershell

Import-Module Microsoft.Graph.Mail

# A UPN can also be used as -UserId.
Get-MgUserMailFolder -UserId $userId -Includehiddenfolders true 

```