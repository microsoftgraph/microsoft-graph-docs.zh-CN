---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6fd34cac6e237a97ffc4dc56b72f9e57c9099e9
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615675"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Cancelling for this week due to all hands";

await graphClient.Me.Events["{id}"]
    .Cancel(comment)
    .Request()
    .PostAsync();

```