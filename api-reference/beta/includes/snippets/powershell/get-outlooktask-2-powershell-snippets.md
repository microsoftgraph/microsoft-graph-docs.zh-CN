---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5e41c6b38827fe8c56b4d5bacdaba535d7aa5246
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350298"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserOutlookTask -UserId $userId -OutlookTaskId $outlookTaskId

```