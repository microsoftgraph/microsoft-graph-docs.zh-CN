---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1fb4f03e9437ddd63972a95d86f47ea49b3b08fd
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58266334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .MarkRead(messageIds)
    .Request()
    .PostAsync();

```