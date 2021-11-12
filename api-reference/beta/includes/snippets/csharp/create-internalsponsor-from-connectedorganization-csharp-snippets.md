---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a2e43eea38a3484f861e9cb0cefc4bbc974dd552aabecb7290695b5cff083a68
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161576"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].InternalSponsors.References
    .Request()
    .AddAsync(directoryObject);

```