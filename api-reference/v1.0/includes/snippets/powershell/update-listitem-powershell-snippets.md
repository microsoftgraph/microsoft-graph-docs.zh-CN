---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 34ebc4d8d26c9c77173671755ddc5e231b997c7c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132493"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Color = "Fuchsia"
    Quantity = 
}

Update-MgSiteListItemField -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```