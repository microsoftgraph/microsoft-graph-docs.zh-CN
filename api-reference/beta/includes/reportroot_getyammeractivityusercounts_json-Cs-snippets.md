---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8f4f76b3fe770413b516cca0ff20740ceb55256e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481721"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerActivityUserCounts = await graphClient.Reports.GetYammerActivityUserCounts('D7')
    .Request()
    .GetAsync();

```