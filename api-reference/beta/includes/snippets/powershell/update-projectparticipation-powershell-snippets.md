---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28633b7211c768b9420fe9265409cd7e033d9bc2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350974"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    AllowedAudiences = "organization"
    Client = @{
        Department = "Corporate Marketing"
        WebUrl = "https://www.contoso.com"
    }
}

# A UPN can also be used as -UserId.
Update-MgUserProfileProject -UserId $userId -ProjectParticipationId $projectParticipationId -BodyParameter $params

```