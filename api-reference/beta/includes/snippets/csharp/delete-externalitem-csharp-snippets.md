---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f529621be92f29f5db209bf6fe8168f0e906e09
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006782"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Connections["contosohr"].Items["TSP228082938"]
    .Request()
    .DeleteAsync();

```