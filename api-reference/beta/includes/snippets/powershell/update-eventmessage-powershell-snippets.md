---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4bd142df2a66ac6ad680db9ebc2f80ea2625b2f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351315"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    IsRead = "true"
}

# A UPN can also be used as -UserId.
Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```