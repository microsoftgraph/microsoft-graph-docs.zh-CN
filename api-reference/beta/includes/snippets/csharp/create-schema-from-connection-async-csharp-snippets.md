---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec0e908da148e6541d2644f689c15411c9c37d08
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516041"
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
    .AddAsync(schema);

```