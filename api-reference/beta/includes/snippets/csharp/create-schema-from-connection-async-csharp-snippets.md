---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67d516e7d088dd5fbe9da04bd6d6405b0d4cd4f2
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45008643"
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
            IsRefinable = true,
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

await graphClient.Connections["contosohr"].Schema
    .Request()
    .Header("Prefer","respond-async")
    .AddAsync(schema);

```