---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f30312fb8230fcc44fe69ce6e6e54c2edd4af4a
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47938416"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new ExternalItem
{
    Acl = new List<Acl>()
    {
        new Acl
        {
            Type = AclType.User,
            Value = "49103559-feac-4575-8b94-254814dfca72",
            AccessType = AccessType.Deny,
            IdentitySource = "azureActiveDirectory"
        }
    },
    Properties = new Properties
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"title", "Error in the payment gateway"},
            {"priority", "1"},
            {"assignee", "john@contoso.com"}
        }
    },
    Content = new ExternalItemContent
    {
        Value = "<h1>Error in payment gateway</h1><p>Error details...</p>",
        Type = ExternalItemContentType.Html
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .PutAsync(externalItem);

```