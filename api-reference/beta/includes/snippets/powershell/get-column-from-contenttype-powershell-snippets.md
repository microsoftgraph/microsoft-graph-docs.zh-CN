---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3cfed425b501bd75bcf6d0ab902249f20b293e8b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62125935"
---
```powershell

Import-Module Microsoft.Graph.Sites

Get-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId -ColumnDefinitionId $columnDefinitionId

```