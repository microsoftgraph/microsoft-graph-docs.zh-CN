---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4230b4d478ad0b69657ac66f74adb2e00e0aa7ae
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735003"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .TentativelyAccept(comment,sendResponse)
    .Request()
    .PostAsync();

```