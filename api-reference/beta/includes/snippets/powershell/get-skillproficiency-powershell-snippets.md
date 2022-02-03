---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0c22cdb6eb88c67b73a77dfb615af53995769940
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350788"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId

```