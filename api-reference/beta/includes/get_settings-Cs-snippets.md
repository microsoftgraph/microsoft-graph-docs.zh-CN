---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 76a687d6c802325a064108e81c253f738c44e6d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446083"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var settings = await graphClient.Settings
    .Request()
    .GetAsync();

```