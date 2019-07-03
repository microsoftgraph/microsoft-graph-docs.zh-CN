---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 06bf68b823d4c914b7c48419dbfba545f52cc8f9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35478294"
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