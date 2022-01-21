---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1582fa5023c41a38b90a9da5bb884570845b86ea
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126326"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItemVersion -SiteId $siteId -ListId $listId -ListItemId $listItemId -ListItemVersionId $listItemVersionId -ExpandProperty "fields" 

```