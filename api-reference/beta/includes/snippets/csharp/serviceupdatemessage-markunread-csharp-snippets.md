---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a3f70221242e7b6ffd8a47cc2e7b80fd67c0ed9
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210792"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .MarkUnread(messageIds)
    .Request()
    .PostAsync();

```