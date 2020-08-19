---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a830b3d202d2933dc184207c5da22b0f337e8582
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810247"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{connectedOrganizationId}"].InternalSponsors["{id}"].Reference
    .Request()
    .DeleteAsync();

```