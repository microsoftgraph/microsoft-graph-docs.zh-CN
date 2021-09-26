---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bd0c11c7a5e3ddf766a1ee0aec797a93d832c2fbdc0f98f9b517b947cc6002c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcUserSetting = await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .Expand("assignments")
    .GetAsync();

```