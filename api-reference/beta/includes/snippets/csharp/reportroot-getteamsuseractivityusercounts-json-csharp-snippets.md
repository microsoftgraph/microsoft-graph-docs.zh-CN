---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a95443822db21a5b49f4b572c00ba01808a6c6bc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35479979"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getTeamsUserActivityUserCounts = await graphClient.Reports.GetTeamsUserActivityUserCounts('D7')
    .Request()
    .GetAsync();

```