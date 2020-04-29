---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1d63173f62f485228138b1d4c75b804698e10f37
ms.sourcegitcommit: 9b507499fb1ec61b4de47f36f915ae29c8594459
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2020
ms.locfileid: "43935210"
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
            IdentitySource = "Azure Active Directory"
        }
    },
    Properties = new Properties
    {
        Title = "Error in the payment gateway",
        Priority = 1,
        Assignee = "john@contoso.com"
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