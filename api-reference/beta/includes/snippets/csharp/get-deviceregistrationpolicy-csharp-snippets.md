---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c4b42cbc682df8da2aaeabc0fd789cae61276500
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2022
ms.locfileid: "65694815"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deviceRegistrationPolicy = await graphClient.Policies.DeviceRegistrationPolicy
    .Request()
    .GetAsync();

```