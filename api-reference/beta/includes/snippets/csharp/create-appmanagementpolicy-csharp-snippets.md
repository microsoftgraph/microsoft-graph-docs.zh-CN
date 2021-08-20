---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7825ccefb122e353a392dca05841188c2a07a719
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262386"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var appManagementPolicy = new AppManagementPolicy
{
    DisplayName = "Credential management policy",
    Description = "Cred policy sample",
    IsEnabled = true,
    Restrictions = new AppManagementConfiguration
    {
        PasswordCredentials = new List<PasswordCredentialConfiguration>()
        {
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.PasswordAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2019-10-19T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.PasswordLifetime,
                MaxLifetime = new Duration("P4DT12H30M5S"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2018-10-19T10:37:00Z")
            }
        }
    }
};

await graphClient.Policies.AppManagementPolicies
    .Request()
    .AddAsync(appManagementPolicy);

```