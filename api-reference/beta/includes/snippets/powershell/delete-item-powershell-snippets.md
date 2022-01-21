---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 24590dd0f1c998a7e127bcae43132d5e07c6311e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62116050"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteListItem -SiteId $siteId -ListId $listId -ListItemId $listItemId

```