---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 660b51a049795432e9a88b19fa128407c8d7f9d9
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101340"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteContentType -SiteId $siteId -ContentTypeId $contentTypeId

```