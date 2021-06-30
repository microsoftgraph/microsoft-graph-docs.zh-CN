---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7d54f0c371fc012329f60edc460a95814ec244f
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209299"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Unfavorite(messageIds)
    .Request()
    .PostAsync();

```