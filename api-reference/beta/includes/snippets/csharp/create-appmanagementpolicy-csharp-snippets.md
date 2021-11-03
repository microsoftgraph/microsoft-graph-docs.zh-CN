---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 92fa36a806ac02bf0c825a03ffd178701ae51663
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60690105"
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
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2014-10-19T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyAddition,
                MaxLifetime = null,
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2019-10-19T10:37:00Z")
            },
            new PasswordCredentialConfiguration
            {
                RestrictionType = AppCredentialRestrictionType.SymmetricKeyLifetime,
                MaxLifetime = new Duration("P4D"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2014-10-19T10:37:00Z")
            }
        },
        KeyCredentials = new List<KeyCredentialConfiguration>()
        {
            new KeyCredentialConfiguration
            {
                RestrictionType = AppKeyCredentialRestrictionType.AsymmetricKeyLifetime,
                MaxLifetime = new Duration("P90D"),
                RestrictForAppsCreatedAfterDateTime = DateTimeOffset.Parse("2014-10-19T10:37:00Z")
            }
        }
    }
};

await graphClient.Policies.AppManagementPolicies
    .Request()
    .AddAsync(appManagementPolicy);

```