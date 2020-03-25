---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: edde0e3f17002edc750be89ad4d2271bd84b3182
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].AllowedUsers["{id}"].Reference
    .Request()
    .DeleteAsync();

```