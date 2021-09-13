---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e382261f7fe7615a9b3344ff20fb8ed525a310273ec2021126fccbc5fbcbfb11
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279727"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    Id = "my-custom-consent-policy",
    DisplayName = "Custom application consent policy",
    Description = "A custom permission grant policy to customize conditions for granting consent."
};

await graphClient.Policies.PermissionGrantPolicies
    .Request()
    .AddAsync(permissionGrantPolicy);

```