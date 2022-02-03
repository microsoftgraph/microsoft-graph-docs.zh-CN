---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ecaaae075e255d119b89df4ceda41b0167fda00
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348978"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    SourceFile = @{
        SharepointIds = @{
            ListId = "e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0"
            ListItemId = "2"
        }
    }
    DestinationFileName = "newname.txt"
}

Copy-MgSiteContentTypeToDefaultContentLocation -SiteId $siteId -ContentTypeId $contentTypeId -BodyParameter $params

```