---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1358e9a17025c9df3880f953fc04571f2ee63d75
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135287"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "Lifetime Achievement award from the International Association of Branding Managers"
    DisplayName = "Lifetime Achievement Award For Excellence in Branding"
    IssuedDate = "Date"
    IssuingAuthority = "International Association of Branding Management"
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
    WebUrl = "https://www.iabm.io"
}

New-MgUserProfileAward -UserId $userId -BodyParameter $params

```