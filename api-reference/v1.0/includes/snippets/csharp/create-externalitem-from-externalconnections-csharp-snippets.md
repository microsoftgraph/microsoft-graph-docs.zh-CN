---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9343f7a95cd50eb1e4d740823b9f21267013fd173bbd54c4f175377707af71df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902274"
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