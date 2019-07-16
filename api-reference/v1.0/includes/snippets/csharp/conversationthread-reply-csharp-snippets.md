---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e91951eaed9c0ef39792bd4ec47b6582912d9531
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738238"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    }
};

await graphClient.Groups["{id}"].Threads["{id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```