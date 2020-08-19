---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cd9cb4bf4cbb90c1697617753d32beab8cfad18e
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810112"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"].InternalSponsors.References
    .Request()
    .AddAsync(directoryObject);

```