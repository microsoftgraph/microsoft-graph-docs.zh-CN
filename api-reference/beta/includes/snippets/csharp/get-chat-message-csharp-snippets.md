---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 9ff0d8deaedce2e902dda3193b463de3c7cff781
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35863557"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = await graphClient.Me.Chats["{id}"].Messages["{id}"]
    .Request()
    .GetAsync();

```