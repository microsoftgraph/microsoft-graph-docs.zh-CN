---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0da606610bd01e5fd2ec502f28fd5e861c4a550ec19a7829a2b00ad9bf759ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106926"
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