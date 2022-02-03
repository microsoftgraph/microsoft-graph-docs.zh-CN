---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d22ae312ed984c0cdcd6f36b279201f7fa41c7db
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349174"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Type = "embed"
}

New-MgSiteListItemLink -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```