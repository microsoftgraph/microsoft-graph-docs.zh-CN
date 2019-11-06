---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3e2bc3ba8047fe37839b3f82473f9e7416ba75f9
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994544"
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
    Content = "Textual content of the file"
};

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .PutAsync(externalItem);

```