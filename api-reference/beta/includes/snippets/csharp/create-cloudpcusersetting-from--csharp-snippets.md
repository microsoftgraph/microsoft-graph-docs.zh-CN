---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3980b41aa9aceade9f536f28d3b5ff1a0239f973
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = new CloudPcUserSetting
{
    DisplayName = "Example",
    SelfServiceEnabled = false,
    LocalAdminEnabled = true
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings
    .Request()
    .AddAsync(cloudPcUserSetting);

```