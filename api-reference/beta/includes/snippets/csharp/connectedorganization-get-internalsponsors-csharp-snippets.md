---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b05489db0ca369374ea8e2362c7f0b6be3943f9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810155"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var internalSponsors = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"].InternalSponsors
    .Request()
    .GetAsync();

```