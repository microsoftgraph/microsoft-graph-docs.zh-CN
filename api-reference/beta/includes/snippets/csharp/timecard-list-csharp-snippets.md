---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd7d67b0fb7a8d6ee7ff6b0749d541cb0faab37f
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870680"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeCards = await graphClient.Teams["{team-id}"].Schedule.TimeCards
    .Request()
    .Filter("state eq 'clockedOut'")
    .Top(2)
    .GetAsync();

```