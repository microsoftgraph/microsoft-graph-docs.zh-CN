---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ddab80df12271e0c2e133c3e2b70e86ef8622da8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = new Schema
{
    BaseType = "microsoft.graph.externalItem",
    Properties = new List<Property>()
    {
        new Property
        {
            Name = "ticketTitle",
            Type = PropertyType.String,
            IsSearchable = true,
            IsRetrievable = true,
            Labels = new List<Label>()
            {
                Label.Title
            }
        },
        new Property
        {
            Name = "priority",
            Type = PropertyType.String,
            IsQueryable = true,
            IsRetrievable = true,
            IsSearchable = false
        },
        new Property
        {
            Name = "assignee",
            Type = PropertyType.String,
            IsRetrievable = true
        }
    }
};

await graphClient.External.Connections["{externalConnection-id}"].Schema
    .Request()
    .Header("Prefer","respond-async")
    .AddAsync(schema);

```