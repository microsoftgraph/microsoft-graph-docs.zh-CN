---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d2780d88f14407a751d16a599601f3df09c40b6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479330"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Properties = new List<ExtensionSchemaProperty>()
    {
        new ExtensionSchemaProperty
        {
            Name = "new-name-value",
            Type = "new-type-value"
        },
        new ExtensionSchemaProperty
        {
            Name = "additional-name-value",
            Type = "additional-type-value"
        }
    }
};

await graphClient.SchemaExtensions["{id}"]
    .Request()
    .UpdateAsync(schemaExtension);

```