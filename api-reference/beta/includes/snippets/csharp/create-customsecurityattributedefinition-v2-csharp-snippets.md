---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef25ec85ad57c187c6c2e3b73b41ded79580e37
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61226797"
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
    UsePreDefinedValuesOnly = true
};

await graphClient.Directory.CustomSecurityAttributeDefinitions
    .Request()
    .AddAsync(customSecurityAttributeDefinition);

```