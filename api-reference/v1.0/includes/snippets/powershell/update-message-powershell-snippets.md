---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b59172657d75a9092bd6cc2d51ed96b85cc6f0f
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350157"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    Subject = "subject-value"
    Body = @{
        ContentType = ""
        Content = "content-value"
    }
    InferenceClassification = "other"
}

# A UPN can also be used as -UserId.
Update-MgUserMessage -UserId $userId -MessageId $messageId -BodyParameter $params

```