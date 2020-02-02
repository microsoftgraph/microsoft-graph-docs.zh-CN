---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: be522034fc6c17a23df04492630a61f75290b82e
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37045337"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .TentativelyAccept(sendResponse,comment)
    .Request()
    .PostAsync();

```