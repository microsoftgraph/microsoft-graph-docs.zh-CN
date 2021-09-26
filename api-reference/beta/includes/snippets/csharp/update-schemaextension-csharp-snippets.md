---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 898fd9094b6cdb1660ac2c8ead3ad7150c4e3783
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767312"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schemaExtension = new SchemaExtension
{
    Owner = "ef4cb9a8-97c3-4ca7-854b-5cb5ced376fa",
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
        },
        new ExtensionSchemaProperty
        {
            Name = "courseSupervisors",
            Type = "String"
        }
    }
};

await graphClient.SchemaExtensions["{schemaExtension-id}"]
    .Request()
    .UpdateAsync(schemaExtension);

```