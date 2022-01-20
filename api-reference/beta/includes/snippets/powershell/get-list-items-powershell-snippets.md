---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 002362f95c7478ebb69cef3fb456c1cf59c12900
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096278"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteListItem -SiteId $siteId -ListId $listId -ExpandProperty "fields(select=Name,Color,Quantity)" 

```