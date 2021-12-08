---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 52af9f1b4eb765a5bc4926b97a231563b3768e4b
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61336085"
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
    .UpdateAsync(schema);

```