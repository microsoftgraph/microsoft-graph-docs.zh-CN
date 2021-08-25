---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22e7d3e52e94b382b96765c059f7110271f8d752
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tenantAppManagementPolicy = new TenantAppManagementPolicy
{
    IsEnabled = true,
    ApplicationRestrictions = new AppManagementConfiguration
    {
        PasswordCredentials = new List<PasswordCredentialConfiguration>()
        {
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.PasswordAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-04-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.PasswordLifetime,
                MaxLifetime = new Duration("P4DT12H30M5S"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2019-01-01T10:37:00Z")
            }
        }
    }
};

await graphClient.Policies.DefaultAppManagementPolicy
    .Request()
    .UpdateAsync(tenantAppManagementPolicy);

```