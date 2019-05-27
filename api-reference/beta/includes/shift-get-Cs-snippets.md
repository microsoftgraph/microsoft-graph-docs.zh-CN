---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4c9d17e1931bcfe80229c5ca8fe641d2009ba139
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .GetAsync();

```