---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 82dfa20c78e5e4be7ee7c0ba9b08090d51520800
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365GroupsActivityCounts('D7')
    .Request()
    .GetAsync();

```