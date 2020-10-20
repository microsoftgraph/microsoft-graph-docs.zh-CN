---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 159d0f971ddbd981191414e05eb60d322a99a03d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611178"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerBucket = await graphClient.Planner.Buckets["hsOf2dhOJkqyYYZEtdzDe2QAIUCR"]
    .Request()
    .GetAsync();

```