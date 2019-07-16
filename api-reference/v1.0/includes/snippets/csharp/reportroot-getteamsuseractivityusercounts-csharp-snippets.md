---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ce5550bee3eb2891a59d7555733aa28ccec62319
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35738072"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsUserActivityUserCounts('D7')
    .Request()
    .GetAsync();

```