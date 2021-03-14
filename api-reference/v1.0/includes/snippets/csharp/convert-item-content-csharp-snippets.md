---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 042dd411c7e438b49206c2cd092bb0134b21453b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802216"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("format", "{format}")
};

var stream = await graphClient.Me.Drive.Items["{driveItem-id}"].Content
    .Request( queryOptions )
    .GetAsync();

```