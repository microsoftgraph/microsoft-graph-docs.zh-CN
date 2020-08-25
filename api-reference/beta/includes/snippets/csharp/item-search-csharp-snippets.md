---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 487f3bd1f422d3e74215beef9231198cdf0f739f
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873817"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var search = await graphClient.Me.Drive.Root
    .Search("Contoso Projec}")
    .Request()
    .GetAsync();

```