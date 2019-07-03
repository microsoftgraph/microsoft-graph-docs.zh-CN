---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 97ec46bb649c0cb899245cd336dbb8e08e374bfc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35521154"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationId = "destinationId-value";

await graphClient.Me.Messages["{id}"]
    .Copy(destinationId)
    .Request()
    .PostAsync();

```