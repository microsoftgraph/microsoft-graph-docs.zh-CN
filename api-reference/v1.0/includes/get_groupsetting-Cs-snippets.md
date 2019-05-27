---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 20efc75d238e06b807e50b22e2332f2974900902
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupSetting = await graphClient.GroupSettings["{id}"]
    .Request()
    .GetAsync();

```