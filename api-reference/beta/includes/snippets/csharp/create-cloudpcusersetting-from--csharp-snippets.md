---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5af981724e51682e07646082282128ff07c29d6f4809f84e7e8a4a92c23e82f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104649"
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