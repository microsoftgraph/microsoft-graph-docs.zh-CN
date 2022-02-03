---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f3d177ba34b98bf59948c80aabab21b6f8f4658
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341433"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Send-MgUserMessage -UserId $userId -MessageId $messageId

```