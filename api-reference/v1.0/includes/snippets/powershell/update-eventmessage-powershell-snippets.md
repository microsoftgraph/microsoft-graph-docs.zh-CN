---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 83e8a3ae1dbf9ca6fc2e23b708f1833d0ae59ff6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351432"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    IsRead = $true
}

# A UPN can also be used as -UserId.
Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```