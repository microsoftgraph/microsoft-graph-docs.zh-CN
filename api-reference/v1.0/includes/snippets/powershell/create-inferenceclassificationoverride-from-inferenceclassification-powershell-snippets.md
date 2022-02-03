---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de3d1a877489c2610f0aad2ce0ff95ff0ac42102
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352464"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ClassifyAs = "focused"
    SenderEmailAddress = @{
        Name = "Samantha Booth"
        Address = "samanthab@adatum.onmicrosoft.com"
    }
}

# A UPN can also be used as -UserId.
New-MgUserInferenceClassificationOverride -UserId $userId -BodyParameter $params

```