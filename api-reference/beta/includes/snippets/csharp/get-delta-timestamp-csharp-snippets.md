---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15116730c83ab50ae3ca7d663bae7ac5705a785f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61019924"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("token", "2021-09-29T20:00:00Z")
};

var delta = await graphClient.Me.Drive.Root
    .Delta()
    .Request( queryOptions )
    .GetAsync();

```