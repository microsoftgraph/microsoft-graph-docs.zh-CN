---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fce168085e011bcceceba21f884c95fc792be42a
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947977"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"]
    .GetCapabilities()
    .Request()
    .PostAsync();

```