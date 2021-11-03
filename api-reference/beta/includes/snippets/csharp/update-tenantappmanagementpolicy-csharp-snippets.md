---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2894e1fddc6308c3b9fb8022055f183aa8f15836
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696096"
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
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2021-04-01T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyLifetime,
                MaxLifetime = new Duration("P40D"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2015-04-01T10:37:00Z")
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