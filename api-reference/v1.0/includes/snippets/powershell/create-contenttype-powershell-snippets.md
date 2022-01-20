---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 643a2f8593d77a2a7d8d64c3858db6a39ec42513
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110613"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Name = "docSet"
    Description = "custom docset"
    Base = @{
        Name = "Document Set"
        Id = "0x0120D520"
    }
    Group = "Document Set Content Types"
}

New-MgSiteContentType -SiteId $siteId -BodyParameter $params

```