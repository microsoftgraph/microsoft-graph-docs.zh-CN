---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42f7254271102fe08346a2faccfefbe0b8642eb0
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351640"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    CertificationId = "KB-1235466333663322"
    Description = "Blackbelt in Marketing - Brand Management"
    DisplayName = "Marketing Blackbelt - Brand Management"
    ThumbnailUrl = "https://iame.io/dfhdfdfd334.jpg"
    WebUrl = "https://www.iame.io/blackbelt"
}

# A UPN can also be used as -UserId.
New-MgUserProfileCertification -UserId $userId -BodyParameter $params

```