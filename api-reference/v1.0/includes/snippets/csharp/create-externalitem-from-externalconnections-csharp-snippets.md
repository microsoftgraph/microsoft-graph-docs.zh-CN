---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09018dce5568970d548c30f5e0f7971052ba1b27
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60688118"
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

await graphClient.External.Connections["{externalConnectors.externalConnection-id}"].Items["{externalConnectors.externalItem-id}"]
    .Request()
    .PutAsync(externalItem);

```