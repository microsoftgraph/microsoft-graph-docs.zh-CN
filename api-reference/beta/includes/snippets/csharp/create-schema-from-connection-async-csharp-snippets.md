---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0d2b584c37fbd6b71ff6418ad3147601dcd0c844b017c456950f78ddb738b700
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220289"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schema = new Microsoft.Graph.ExternalConnectors.Schema
{
    BaseType = "microsoft.graph.externalItem",
    Properties = new List<Microsoft.Graph.ExternalConnectors.Property>()
    {
        new Microsoft.Graph.ExternalConnectors.Property
        {
            Name = "ticketTitle",
            Type = Microsoft.Graph.ExternalConnectors.PropertyType.String,
            IsSearchable = true,
            IsRetrievable = true,
            Labels = new List<Microsoft.Graph.ExternalConnectors.Label>()
            {
                Microsoft.Graph.ExternalConnectors.Label.Title
            }
        },
        new Microsoft.Graph.ExternalConnectors.Property
        {
            Name = "priority",
            Type = Microsoft.Graph.ExternalConnectors.PropertyType.String,
            IsQueryable = true,
            IsRetrievable = true,
            IsSearchable = false
        },
        new Microsoft.Graph.ExternalConnectors.Property
        {
            Name = "assignee",
            Type = Microsoft.Graph.ExternalConnectors.PropertyType.String,
            IsRetrievable = true
        }
    }
};

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Schema
    .Request()
    .Header("Prefer","respond-async")
    .AddAsync(schema);

```