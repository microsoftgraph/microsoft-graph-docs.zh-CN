---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1226321bf834c76df87d1b6f1dfb26ba8c4a7719
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209130"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var messageIds = new List<String>()
{
    "MC172851",
    "MC167983"
};

await graphClient.Admin.ServiceAnnouncement.Messages
    .Unarchive(messageIds)
    .Request()
    .PostAsync();

```