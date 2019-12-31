---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cb4d586b5940130517114ddc73f10f92add181f
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40911636"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessPackageResourceRoles = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["15d889df-3eb8-4e9b-bfb4-b1908849aec4"].AccessPackageResourceRoles
    .Request()
    .Filter("(originSystem+eq+'AadGroup'+and+accessPackageResource/id+eq+'a35bef72-a8aa-4ca3-af30-f6b2ece7208f'),")
    .Expand("accessPackageResource/id+eq+%27a35bef72-a8aa-4ca3-af30-f6b2ece7208f%27)")
    .GetAsync();

```