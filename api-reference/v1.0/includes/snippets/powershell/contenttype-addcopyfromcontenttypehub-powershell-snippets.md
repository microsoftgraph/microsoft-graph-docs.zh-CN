---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22c169fcf5bb26aedc32bcdc4d16283b2dcbc703
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444061"
---
```powershell

Import-Module Microsoft.Graph.Sites

$params = @{
    ContentTypeId = "0x0101"
}

Add-MgSiteListContentTypeCopyFromContentTypeHub -SiteId $siteId -ListId $listId -BodyParameter $params

```