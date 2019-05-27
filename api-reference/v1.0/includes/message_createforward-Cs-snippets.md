---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0ad8a5cb36b21cf6c88a9fd8000f9ba8bc4bd597
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455486"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Messages["{id}"]
    .CreateForward()
    .Request()
    .PostAsync();

```