---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 809d5603e3f2883ec1d4b09eff2af9d9e8e802c3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352060"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    Description = "One persons journey to the top of the branding management field."
    DisplayName = "Got Brands? The story of Innocenty Popov and his journey to the top."
    PublishedDate = "Date"
    Publisher = "International Association of Branding Management Publishing"
    ThumbnailUrl = "https://iabm.io/sdhdfhsdhshsd.jpg"
    WebUrl = "https://www.iabm.io"
}

# A UPN can also be used as -UserId.
New-MgUserProfilePublication -UserId $userId -BodyParameter $params

```