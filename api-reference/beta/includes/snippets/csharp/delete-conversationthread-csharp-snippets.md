---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 070506d6496492be405a4e7691c0fcf4bbebb908
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607783"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .DeleteAsync();

```