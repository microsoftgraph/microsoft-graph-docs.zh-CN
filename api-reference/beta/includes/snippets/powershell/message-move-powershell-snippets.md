---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7a82c6e58945d2ccd4eee78dea2cda0701571ae3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341615"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    DestinationId = "deleteditems"
}

# A UPN can also be used as -UserId.
Move-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```