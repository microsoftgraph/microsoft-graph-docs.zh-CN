---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4ddaa51f960fd65909793ac85e1b609212ff2830
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948257"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var services = await graphClient.Print.Services
    .Request()
    .GetAsync();

```