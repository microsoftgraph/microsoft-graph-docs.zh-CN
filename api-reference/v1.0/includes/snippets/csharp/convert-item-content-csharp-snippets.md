---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 78e0dea1220686cb1bc2cbc065586784961c586b
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Me.Drive.Items["{item-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```