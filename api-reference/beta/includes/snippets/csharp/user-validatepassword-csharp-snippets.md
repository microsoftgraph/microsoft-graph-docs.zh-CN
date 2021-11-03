---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5d4d4d234cd4e3b6b7730c1e9651dac8b3f8a271
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729960"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var password = "1234567890";

await graphClient.Users
    .ValidatePassword(password)
    .Request()
    .PostAsync();

```