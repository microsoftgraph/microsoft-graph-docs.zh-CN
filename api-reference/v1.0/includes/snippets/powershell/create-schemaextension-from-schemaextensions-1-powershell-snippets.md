---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 210e007dd3432d0d7e891945c053030f031feedd
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091759"
---
```powershell

Import-Module Microsoft.Graph.SchemaExtensions

$params = @{
    Id = "graphlearn_courses"
    Description = "Graph Learn training courses extensions"
    TargetTypes = @(
        "Group"
    )
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