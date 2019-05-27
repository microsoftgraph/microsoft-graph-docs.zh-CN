---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 06bf68b823d4c914b7c48419dbfba545f52cc8f9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var sendResponse = true;

await graphClient.Me.Events["{id}"]
    .Accept(comment,sendResponse)
    .Request()
    .PostAsync();

```