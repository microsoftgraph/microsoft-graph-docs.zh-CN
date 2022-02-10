---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a730e49768b07a048d401ba0c2d8c7e5a3600fc9
ms.sourcegitcommit: 4e16f26b6b685a6a3dae855a04979c84105609b9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/10/2022
ms.locfileid: "62519334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var customSecurityAttributeDefinition = new CustomSecurityAttributeDefinition
{
    AttributeSet = "Engineering",
    Description = "Active projects for user",
    IsCollection = true,
    IsSearchable = true,
    Name = "Project",
    Status = "Available",
    Type = "String",
    UsePreDefinedValuesOnly = true,
    AllowedValues = new CustomSecurityAttributeDefinitionAllowedValuesCollectionPage()
    {
        new AllowedValue
        {
            Id = "Alpine",
            IsActive = true
        },
        new AllowedValue
        {
            Id = "Baker",
            IsActive = true
        },
        new AllowedValue
        {
            Id = "Cascade",
            IsActive = true
        }
    }
};

await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .AddAsync(customSecurityAttributeDefinition);

```