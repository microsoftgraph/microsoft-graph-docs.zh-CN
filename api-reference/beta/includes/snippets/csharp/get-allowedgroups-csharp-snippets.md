---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 467eaa5ae02c0362ea2a342aab980a5ad07286fa
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947919"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var allowedGroups = await graphClient.Print.Printers["{id}"].AllowedGroups
    .Request()
    .GetAsync();

```