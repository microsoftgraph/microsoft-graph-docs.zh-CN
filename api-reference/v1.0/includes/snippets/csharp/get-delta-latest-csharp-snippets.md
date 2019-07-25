---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 33a10630411230cc5e9fd5ab855f3e129cc3de64
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35891016"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("token", "latest")
};

var delta = await graphClient.Me.Drive.Root
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```