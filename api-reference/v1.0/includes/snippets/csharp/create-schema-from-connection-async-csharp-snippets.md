---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c771a97f2c445b85e65ea9c09276089062fe7321
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53580713"
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