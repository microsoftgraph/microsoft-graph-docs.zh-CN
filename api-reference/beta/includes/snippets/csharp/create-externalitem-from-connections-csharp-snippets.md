---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f027dcc1241aaa2d7543b3fe336d79084df325eb
ms.sourcegitcommit: c7776e5659c391e7c9ce1cd46e242a5ddc38dba2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/01/2021
ms.locfileid: "51491005"
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

await graphClient.External.Connections["{externalConnection-id}"].Items["{externalItem-id}"]
    .Request()
    .PutAsync(externalItem);

```
