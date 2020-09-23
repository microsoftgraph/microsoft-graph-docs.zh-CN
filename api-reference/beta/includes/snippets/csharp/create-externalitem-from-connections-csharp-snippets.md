---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9e10a6264c635c8ce2ed82d9fea13dd825916c6
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48230699"
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
            Value = "e811976d-83df-4cbd-8b9b-5215b18aa874",
            AccessType = AccessType.Grant,
            IdentitySource = "azureActiveDirectory"
        },
        new Acl
        {
            Type = AclType.Group,
            Value = "14m1b9c38qe647f6a",
            AccessType = AccessType.Deny,
            IdentitySource = "external"
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
        Value = "Error in payment gateway...",
        Type = ExternalItemContentType.Text
    }
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .PutAsync(externalItem);

```