---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d7da5d0b68c2703a3ff2e19f5f4933ab055de66d
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351064"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId

```