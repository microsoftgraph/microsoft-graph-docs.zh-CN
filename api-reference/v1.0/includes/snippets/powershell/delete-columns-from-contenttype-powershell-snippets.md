---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3640f8bfa5ce760e75bd59a70c2ce35f5ed5992
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62128931"
---
```powershell

Import-Module Microsoft.Graph.Sites

Remove-MgSiteContentTypeColumn -SiteId $siteId -ContentTypeId $contentTypeId -ColumnDefinitionId $columnDefinitionId

```