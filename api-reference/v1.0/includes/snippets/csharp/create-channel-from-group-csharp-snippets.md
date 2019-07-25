---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cac770ea5ab74c855869e626b57a9828b1205ac5
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734192"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "Architecture Discussion",
    Description = "This channel is where we debate all future architecture plans"
};

await graphClient.Teams["{id}"].Channels
    .Request()
    .AddAsync(channel);

```