---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bb4f3a89ccef1f8e5581e3a64d4aa41a209229e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105425"
---
```powershell

Import-Module Microsoft.Graph.SchemaExtensions

$params = @{
    Id = "courses"
    Description = "Graph Learn training courses extensions"
    TargetTypes = @(
        "Group"
    )
    Owner = "50897f70-a455-4adf-87bc-4cf17091d5ac"
    Properties = @(
        @{
            Name = "courseId"
            Type = "Integer"
        }
        @{
            Name = "courseName"
            Type = "String"
        }
        @{
            Name = "courseType"
            Type = "String"
        }
    )
}

New-MgSchemaExtension -BodyParameter $params

```