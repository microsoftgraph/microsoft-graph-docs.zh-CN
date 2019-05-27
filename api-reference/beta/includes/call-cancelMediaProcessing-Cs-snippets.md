---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea35d4442b48be4ef2502fcbecf5065a395032db
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34456334"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var all = true;

var clientContext = "clientContext-value";

await graphClient.App.Calls["{id}"]
    .CancelMediaProcessing(all,clientContext)
    .Request()
    .PostAsync();

```