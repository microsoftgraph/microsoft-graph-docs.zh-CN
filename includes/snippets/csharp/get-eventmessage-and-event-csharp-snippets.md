---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2edd50a1f6807b65008591f84e7da4929e78b7e
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774644"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = await graphClient.Me.Messages["AAMkADADVj3fyAABZ5hYdAAA="]
    .Request()
    .Expand("eventMessage/event")
    .GetAsync();

```