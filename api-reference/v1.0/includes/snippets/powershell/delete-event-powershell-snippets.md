---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7b3d2440761a7d4c85ea7c8de8ae625e9d35dfef
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349662"
---
```powershell

Import-Module Microsoft.Graph.Calendar

# A UPN can also be used as -UserId.
Remove-MgUserEvent -UserId $userId -EventId $eventId

```