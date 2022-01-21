---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fe9c8fcce1d4c2656719ade493affd3f9c6554c3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132865"
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

New-MgUserProfileCertification -UserId $userId -BodyParameter $params

```