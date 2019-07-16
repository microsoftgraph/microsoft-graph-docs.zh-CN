---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1e368a464a693aaf45e11457c2a8dad12971d199
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739119"
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