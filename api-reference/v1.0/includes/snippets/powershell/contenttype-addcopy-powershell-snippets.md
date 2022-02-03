---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 487aca54a685d09512cba8d87f568597382da0d5
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346738"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    ContentType = "https://graph.microsoft.com/v1.0/sites/{site-id}/contentTypes/0x0101"
}

Add-MgSiteListContentTypeCopy -SiteId $siteId -ListId $listId -BodyParameter $params

```