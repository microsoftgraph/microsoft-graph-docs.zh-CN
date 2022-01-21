---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 034cf81c7bef94e7b1804a01b4f28c8af07e7aab
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62137614"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.Assignments["{accessPackageAssignment-id}"].Target.ConnectedOrganization.InternalSponsors
    .Request()
    .GetAsync();

```