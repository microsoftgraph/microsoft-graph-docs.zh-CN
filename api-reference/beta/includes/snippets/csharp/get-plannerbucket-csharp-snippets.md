---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 159d0f971ddbd981191414e05eb60d322a99a03d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["hsOf2dhOJkqyYYZEtdzDe2QAIUCR"]
    .Request()
    .GetAsync();

```