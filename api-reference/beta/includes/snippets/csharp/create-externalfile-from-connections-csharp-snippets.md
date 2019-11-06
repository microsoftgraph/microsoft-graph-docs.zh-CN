---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 21d838aea92de7dde82ef7ca644df52a69214858
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var externalItem = new ExternalFile
{
    Acl = new List<Acl>()
    {
        new Acl
        {
            Type = AclType.User,
            Value = "49103559-feac-4575-8b94-254814dfca72",
            AccessType = AccessType.Grant,
            IdentitySource = "Azure Active Directory"
        }
    },
    CreatedDateTime = "2019-01-31T03:44:19.0354159Z",
    ModifiedDateTime = "2019-01-31T03:44:19.0354159Z",
    CreatedBy = "Pradeep Gupta",
    LastModifiedBy = "Adele Vance",
    Title = "Enterprise Search Graph Ingestion API",
    Url = "file://filesrv02.corp.contoso.com/data/project/Enterprise Search.docx",
    Name = "Enterprise Search.docx",
    Extension = "docx",
    Size = 8676776,
    Content = "The quick brown fox jumps over the lazy dog."
};

await graphClient.Connections["contosofiles"].Items["myFile01"]
    .Request()
    .PutAsync(externalItem);

```