---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4c866b1154ea8aa68e48c1fd2210f466454cf71
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349425"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId

```