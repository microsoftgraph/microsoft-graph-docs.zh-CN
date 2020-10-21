---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ccc398b5fce5b00095f433340201b708eb0180b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604784"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Id = "courses",
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