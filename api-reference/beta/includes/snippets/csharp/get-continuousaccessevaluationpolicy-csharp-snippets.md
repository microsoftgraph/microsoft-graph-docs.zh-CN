---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0368a7776b571757f975d9da566b054261ab1025
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223229"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var continuousAccessEvaluationPolicy = await graphClient.Identity.ContinuousAccessEvaluationPolicy
    .Request()
    .GetAsync();

```