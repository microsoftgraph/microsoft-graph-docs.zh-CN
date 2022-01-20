---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f1c145e922dec680de68e4542999e64b2cf654b4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105995"
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

New-MgUserInferenceClassificationOverride -UserId $userId -BodyParameter $params

```