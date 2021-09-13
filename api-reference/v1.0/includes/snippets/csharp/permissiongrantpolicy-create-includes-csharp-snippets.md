---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 61c0aec36c0d44c5b51399fc50587c1089d02e483a8ca94cc256121efb15543c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ClientApplicationsFromVerifiedPublisherOnly = true
};

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Includes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```