---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 789f3e12955640b43fb4a15e44cc9c65e52a44f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785462"
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

await graphClient.Connections["{externalConnection-id}"].Items["{externalItem-id}"]
    .Request()
    .PutAsync(externalItem);

```