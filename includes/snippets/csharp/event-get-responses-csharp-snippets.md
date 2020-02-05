---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84f60eba8787486d2159dbb0462e526a7924755e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774646"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var @event = await graphClient.Me.Calendar.Events["AAMkADJXJGu0AABf02qwAAA="]
    .Request()
    .GetAsync();

```