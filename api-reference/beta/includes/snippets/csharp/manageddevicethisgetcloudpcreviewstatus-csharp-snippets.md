---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dca8946fd67adde37fc9fb8e02119a93f8d5b633
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694559"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcReviewStatus = await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .GetCloudPcReviewStatus()
    .Request()
    .GetAsync();

```