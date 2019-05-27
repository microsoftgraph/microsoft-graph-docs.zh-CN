---
description: 自动生成的文件。 不修改
ms.openlocfilehash: e350960691e1e3069ecf9fb1717daa13b99e7a2c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450354"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var attachment = await graphClient.Me.Events["{id}"].Attachments["{id}"]
    .Request()
    .GetAsync();

```