---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1cf848b072f31af794d964a7a41806df2bec8cb1
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectors = await graphClient.Print.Printers["{id}"].Connectors
    .Request()
    .GetAsync();

```