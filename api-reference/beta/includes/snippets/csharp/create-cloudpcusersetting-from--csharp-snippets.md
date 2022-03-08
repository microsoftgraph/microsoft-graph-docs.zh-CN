---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f10406232552931be743f1ede77f163332c2f53
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = new CloudPcUserSetting
{
    DisplayName = "Example",
    SelfServiceEnabled = false,
    LocalAdminEnabled = true,
    RestorePointSetting = new CloudPcRestorePointSetting
    {
        FrequencyInHours = 16,
        UserRestoreEnabled = true
    }
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings
    .Request()
    .AddAsync(cloudPcUserSetting);

```