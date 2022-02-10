---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff48b4d7ab0f873aaf34ccb8116b258a17139d8d
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519362"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AttributeSet = "Engineering"
    Description = "Active projects for user"
    IsCollection = $true
    IsSearchable = $true
    Name = "Project"
    Status = "Available"
    Type = "String"
    UsePreDefinedValuesOnly = $true
    AllowedValues = @(
        @{
            Id = "Alpine"
            IsActive = $true
        }
        @{
            Id = "Baker"
            IsActive = $true
        }
        @{
            Id = "Cascade"
            IsActive = $true
        }
    )
}

New-MgDirectoryCustomSecurityAttributeDefinition -BodyParameter $params

```