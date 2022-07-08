---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3b20bdb46b58a2c854b6c284562beca3cb03f7cf
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65695228"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceRegistrationPolicy = new DeviceRegistrationPolicy
{
    Id = "deviceRegistrationPolicy",
    DisplayName = "Device Registration Policy",
    Description = "Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks",
    UserDeviceQuota = 50,
    MultiFactorAuthConfiguration = MultiFactorAuthConfiguration.NotRequired,
    AzureADRegistration = new AzureADRegistrationPolicy
    {
        AppliesTo = PolicyScope.None,
        IsAdminConfigurable = false,
        AllowedUsers = new List<String>()
        {
        },
        AllowedGroups = new List<String>()
        {
        }
    },
    AzureADJoin = new AzureAdJoinPolicy
    {
        AppliesTo = PolicyScope.None,
        IsAdminConfigurable = true,
        AllowedUsers = new List<String>()
        {
        },
        AllowedGroups = new List<String>()
        {
        }
    }
};

await graphClient.DeviceRegistrationPolicy
    .Request()
    .PutAsync(deviceRegistrationPolicy);

```