---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b6737ac447b4ce989d0e510432c60a4e97672495
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081724"
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

await graphClient.External.Connections["contosohr"].Schema
    .Request()
    .Header("Prefer","respond-async")
    .AddAsync(schema);

```