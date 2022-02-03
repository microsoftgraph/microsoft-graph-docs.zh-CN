---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e77418a124f84b2ab19fb0af6fdf6fbcf53d320
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350959"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Categories = @(
        "Professional"
    )
    Proficiency = "advancedProfessional"
}

# A UPN can also be used as -UserId.
Update-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId -BodyParameter $params

```