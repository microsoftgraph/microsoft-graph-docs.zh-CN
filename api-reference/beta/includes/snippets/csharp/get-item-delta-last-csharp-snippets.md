---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a3a879fe77b39476fb91bcd62b3b5e804fd0262
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root
    .Delta('1230919asd190410jlka')
    .Request()
    .GetAsync();

```