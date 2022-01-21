---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 378e98c0ba4fb2d617e6343c2715eb067b0b3d8e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62104365"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    DefaultLanguageTag = "en-US"
}

Update-MgSiteTermStore -SiteId $siteId -BodyParameter $params

```