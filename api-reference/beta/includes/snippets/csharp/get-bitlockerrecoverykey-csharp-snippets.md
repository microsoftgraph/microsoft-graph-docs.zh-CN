---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb1655b0a56d3445070915d5befe4fa9022849c7
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48222883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var bitlockerRecoveryKey = await graphClient.Bitlocker.RecoveryKeys["b465e4e8-e4e8-b465-e8e4-65b4e8e465b4"]
    .Request()
    .Select("key")
    .GetAsync();

```