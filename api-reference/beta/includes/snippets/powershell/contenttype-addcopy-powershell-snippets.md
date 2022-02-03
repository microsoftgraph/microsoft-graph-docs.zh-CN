---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9d94b71b118a1032671c9311334a6730f4c2cb29
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62344593"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    ContentType = "https://graph.microsoft.com/beta/sites/id/contentTypes/0x0101"
}

Add-MgSiteListContentTypeCopy -SiteId $siteId -ListId $listId -BodyParameter $params

```