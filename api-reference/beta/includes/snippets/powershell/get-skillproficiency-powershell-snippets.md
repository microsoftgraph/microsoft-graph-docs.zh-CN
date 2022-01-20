---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bcc3b94e42f3d3cf7624b67d8a18a35ca89d308
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129414"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId

```