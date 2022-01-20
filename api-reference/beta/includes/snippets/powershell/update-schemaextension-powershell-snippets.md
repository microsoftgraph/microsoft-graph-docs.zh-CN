---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6fde8b8bc713faed72af0efabf69c52967741702
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62098987"
---
```powershell

Import-Module Microsoft.Graph.SchemaExtensions

$params = @{
    Owner = "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa"
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
        @{
            Name = "courseSupervisors"
            Type = "String"
        }
    )
}

Update-MgSchemaExtension -SchemaExtensionId $schemaExtensionId -BodyParameter $params

```