---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 94918c3273206613ffe38207852d8c7b6421a326
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691050"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{id}"].Jobs["{id}"]
    .Abort(null)
    .Request()
    .PostAsync();

```