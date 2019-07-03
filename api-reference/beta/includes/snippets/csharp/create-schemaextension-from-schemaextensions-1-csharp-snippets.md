---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b28495a8098af8032ab4fcdae6a5029bdd6dca2f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Id = "graphlearn_courses",
    Description = "Graph Learn training courses extensions",
    TargetTypes = new List<String>()
    {
        "Group"
    },
    Properties = new List<ExtensionSchemaProperty>()
    {
        new ExtensionSchemaProperty
        {
            Name = "courseId",
            Type = "Integer"
        },
        new ExtensionSchemaProperty
        {
            Name = "courseName",
            Type = "String"
        },
        new ExtensionSchemaProperty
        {
            Name = "courseType",
            Type = "String"
        }
    }
};

await graphClient.SchemaExtensions
    .Request()
    .AddAsync(schemaExtension);

```