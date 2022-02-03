---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 112571a5471b0f6900c6a18e3cfae19baed576e3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342791"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    DestinationId = "destinationId-value"
}

# A UPN can also be used as -UserId.
Copy-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```