---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 934f7500041e5a45552396c44727e6d3a29d2485
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135203"
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

New-MgUserProfilePublication -UserId $userId -BodyParameter $params

```