---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab28f871a69503fa293fcb38283a73c7bfb82a2b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346765"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    HubSiteUrls = @(
        "https://graph.microsoft.com/v1.0/sites/{site-id}"
    )
    PropagateToExistingLists = $false
}

Join-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```