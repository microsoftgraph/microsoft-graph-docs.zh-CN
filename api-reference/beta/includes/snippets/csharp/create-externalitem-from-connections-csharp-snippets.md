---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a1cfbdfaa1089fb5bd16aa2850d7868973b1aaf3a46de614e75e9bbcd1b93b66
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104789"
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
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Grant,
            IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.AzureActiveDirectory
        },
        new Microsoft.Graph.ExternalConnectors.Acl
        {
            Type = Microsoft.Graph.ExternalConnectors.AclType.Group,
            Value = "14m1b9c38qe647f6a",
            AccessType = Microsoft.Graph.ExternalConnectors.AccessType.Deny,
            IdentitySource = Microsoft.Graph.ExternalConnectors.IdentitySourceType.External
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