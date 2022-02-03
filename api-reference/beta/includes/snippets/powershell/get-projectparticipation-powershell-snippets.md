---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8f5aa3f3759413ea2a7e37985eb6c0cdb416dec
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350185"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId

```