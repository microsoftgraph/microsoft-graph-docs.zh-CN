---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c56763ca7fac873f1d2be87ac39b4c8a2fd3c682
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444704"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .ResetUnseenCount()
    .Request()
    .PostAsync();

```