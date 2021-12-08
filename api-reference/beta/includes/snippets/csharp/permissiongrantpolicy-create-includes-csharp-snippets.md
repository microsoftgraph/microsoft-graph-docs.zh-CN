---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 46c6be3d25803ba8e380c54bbaa6ef606ee6b72e
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348786"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    CertifiedClientApplicationsOnly = true
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```