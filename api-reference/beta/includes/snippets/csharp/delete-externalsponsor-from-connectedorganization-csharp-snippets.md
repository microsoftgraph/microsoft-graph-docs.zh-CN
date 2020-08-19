---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa56bce6691602d479118d8c3b92255b70ca3da5
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810283"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganizationId}"].ExternalSponsors["{id}"].Reference
    .Request()
    .DeleteAsync();

```