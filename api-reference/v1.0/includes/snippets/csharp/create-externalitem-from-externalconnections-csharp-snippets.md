---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4bc7681646ac85a8e84d146f84901eac6dd545b4
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53579916"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new Microsoft.Graph.ExternalConnectors.ExternalItem
{
    Acl = new List<Microsoft.Graph.ExternalConnectors.Acl>()
    {
        new Microsoft.Graph.ExternalConnectors.Acl
        {
            Type = Microsoft.Graph.ExternalConnectors.AclType.User,
            Value = "e811976d-83df-4cbd-8b9b-5215b18aa874",
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Grant
        },
        new Microsoft.Graph.ExternalConnectors.Acl
        {
            Type = Microsoft.Graph.ExternalConnectors.AclType.ExternalGroup,
            Value = "14m1b9c38qe647f6a",
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Deny
        }
    },
    Properties = new Microsoft.Graph.ExternalConnectors.Properties
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"title", "Error in the payment gateway"},
            {"priority", "1"},
            {"assignee", "john@contoso.com"}
        }
    },
    Content = new Microsoft.Graph.ExternalConnectors.ExternalItemContent
    {
        Value = "Error in payment gateway...",
        Type = Microsoft.Graph.ExternalConnectors.ExternalItemContentType.Text
    }
};

await graphClient.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .PutAsync(externalItem);

```