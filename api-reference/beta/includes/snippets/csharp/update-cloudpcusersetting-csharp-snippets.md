---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfbfab9e357ccde6f4bc5a78e313a4408b0a97ed
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207800"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = new CloudPcUserSetting
{
    DisplayName = "Example",
    SelfServiceEnabled = true,
    LocalAdminEnabled = false
};

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .UpdateAsync(cloudPcUserSetting);

```