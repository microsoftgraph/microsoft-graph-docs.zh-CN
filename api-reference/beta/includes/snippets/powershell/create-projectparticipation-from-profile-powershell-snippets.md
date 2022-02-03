---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af49e0c5a828c0381b16983e6203526a5ced01ee
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351509"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Branding"
    )
    Client = @{
        DisplayName = "Contoso Ltd."
        Department = "Corporate Marketing"
        WebUrl = "https://www.contoso.com"
    }
    DisplayName = "Contoso Re-branding Project"
    Detail = @{
        Company = @{
            DisplayName = "Adventureworks Inc."
            Department = "Consulting"
            WebUrl = "https://adventureworks.com"
        }
        Description = "Rebranding of Contoso Ltd."
        JobTitle = "Lead PM Rebranding"
        Role = "project management"
        Summary = "A 6 month project to help Contoso rebrand after they were divested from a parent organization."
    }
}

# A UPN can also be used as -UserId.
New-MgUserProfileProject -UserId $userId -BodyParameter $params

```