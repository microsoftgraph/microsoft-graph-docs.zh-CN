---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e368a464a693aaf45e11457c2a8dad12971d199
ms.sourcegitcommit: c0df90d66cb2072848d4bb0bf730c47a601b99ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/29/2019
ms.locfileid: "34536531"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("token", "latest")
};

var delta = await graphClient.Me.Drive.Root.Delta()
    .Request( queryOptions )
    .GetAsync();

```