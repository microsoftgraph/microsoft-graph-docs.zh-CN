---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3adba746ab0a76610dd31498f4e449307a90057cb67156abbfdf1bfdbb3802d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104839"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    Id = "{id}"
};

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganization-id}"].ExternalSponsors.References
    .Request()
    .AddAsync(directoryObject);

```