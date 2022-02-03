---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 95978cd8a8532dda7f831d53d0b4a3632a5f63b2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347646"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Invoke-MgDismissUserEventReminder -UserId $userId -EventId $eventId

```