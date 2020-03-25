---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: acd09331b54c398346104ad51a90da72e84085a6
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947695"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.PrinterShares["{id}"]
    .Request()
    .DeleteAsync();

```