---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff399f58755fa7b01ff0b013a4d36c1bb478a17c
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444159"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    Comment = "v1"
    ShouldCaptureMinorVersion = $false
}

New-MgSiteListItemDocumentSetVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -BodyParameter $params

```