---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf6f976c16ca52702ccd7b8d74b001ffe4bbfccf
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62130281"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItemVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId

```