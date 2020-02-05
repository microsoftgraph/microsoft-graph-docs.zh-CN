---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6cdbc9cf91f0a7ff14055c4d55a7745a5296cefa
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774634"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "I will probably be able to make it.";

var sendResponse = true;

await graphClient.Me.Events["AAMkADADVj3fyAABZ5ieyAAA="]
    .TentativelyAccept(sendResponse,comment)
    .Request()
    .PostAsync();

```