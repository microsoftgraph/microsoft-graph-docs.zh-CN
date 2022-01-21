---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76b8d8d34d36257ac4b4d4f7f6e004c9bf5595cb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129428"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileSkill -UserId $userId -SkillProficiencyId $skillProficiencyId

```