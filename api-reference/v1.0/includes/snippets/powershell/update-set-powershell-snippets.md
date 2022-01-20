---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ee253352cf96ce0260b4e61a763b8db865aa155e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62110541"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Description = "mySet"
}

Update-MgSiteTermStoreSet -SiteId $siteId -SetId $setId -BodyParameter $params

```