---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3450de1256cee856253fe4165fd84f404444bf150b68f8346f482def0ffe4102
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57106927"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.DeviceManagement.VirtualEndpoint.UserSettings["{cloudPcUserSetting-id}"]
    .Request()
    .DeleteAsync();

```