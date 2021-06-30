---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3fea6d5318d8b140bbae3c57a617b445d369819f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208377"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var userSettings = await graphClient.DeviceManagement.VirtualEndpoint.UserSettings
    .Request()
    .GetAsync();

```