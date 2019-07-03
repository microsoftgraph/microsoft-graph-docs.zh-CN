---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5a4b8f0697c1000ceafef237c88289a8ea0e4a35
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Activities["13881113971988980728"]
    .Request()
    .DeleteAsync();

```