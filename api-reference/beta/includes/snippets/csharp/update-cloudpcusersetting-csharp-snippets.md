---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1642f2c27a9904da8da778c0f70e643e3dad24bf
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335477"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = new CloudPcUserSetting
{
    DisplayName = "Example",
    SelfServiceEnabled = true,
    RestorePointSetting = new CloudPcRestorePointSetting
    {
        FrequencyInHours = "16",
        UserRestoreEnabled = true
    },
    LocalAdminEnabled = false
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .UpdateAsync(cloudPcUserSetting);

```