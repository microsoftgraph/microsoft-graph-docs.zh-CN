---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f52614e2f85090b089118a428df283853d37e7eb
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106333"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AttributeSet = "Engineering"
    Description = "Target completion date"
    IsCollection = $false
    IsSearchable = $true
    Name = "ProjectDate"
    Status = "Available"
    Type = "String"
    UsePreDefinedValuesOnly = $false
}

New-MgDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```