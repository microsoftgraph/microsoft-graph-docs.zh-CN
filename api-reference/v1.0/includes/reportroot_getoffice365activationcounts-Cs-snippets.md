---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8891b6c3023ef5485b1865bf6dcdb0f722b96b8a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463317"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetOffice365ActivationCounts()
    .Request()
    .GetAsync();

```