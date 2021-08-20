---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1226321bf834c76df87d1b6f1dfb26ba8c4a7719
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58257371"
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