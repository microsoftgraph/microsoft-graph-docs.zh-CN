---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0e4deb54c63d54ab0ff5cdbed8cbe77d081f606
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351457"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Professional"
    )
    AllowedAudiences = "organization"
    DisplayName = "API Design"
    Proficiency = "generalProfessional"
    CollaborationTags = @(
        "ableToMentor"
    )
}

# A UPN can also be used as -UserId.
New-MgUserProfileSkill -UserId $userId -BodyParameter $params

```