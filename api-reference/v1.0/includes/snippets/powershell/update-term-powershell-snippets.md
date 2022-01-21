---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 361afd7ee8f3651fc7c4177e8d42811e9da29e15
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62121700"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Labels = @(
        @{
            Name = "changedLabel"
            LanguageTag = "en-US"
            IsDefault = $true
        }
    )
}

Update-MgSiteTermStoreSetTerm -SiteId $siteId -SetId $setId -TermId $termId -BodyParameter $params

```