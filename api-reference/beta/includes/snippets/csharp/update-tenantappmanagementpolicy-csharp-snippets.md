---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f445407bcfb96f2226aecbbe2e0609383803d8fd
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394703"
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
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-01-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.PasswordLifetime,
                MaxLifetime = new Duration("P4DT12H30M5S"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2017-01-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-01-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.CustomPasswordAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyLifetime,
                MaxLifetime = new Duration("P40D"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z")
            }
        },
        KeyCredentials = new List<KeyCredentialConfiguration>()
        {
            new KeyCredentialConfiguration
            {
                RestrictionType = AppKeyCredentialRestrictionType.AsymmetricKeyLifetime,
                MaxLifetime = new Duration("P30D"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-01-01T10:37:00Z")
            }
        }
    }
};

await graphClient.Policies.DefaultAppManagementPolicy
    .Request()
    .UpdateAsync(tenantAppManagementPolicy);

```