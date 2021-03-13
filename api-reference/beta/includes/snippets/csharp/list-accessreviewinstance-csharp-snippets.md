---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dfd2959d932321a35d0c11890075f707c5aa498e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784206"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances
    .Request()
    .Skip(0)
    .Top(100)
    .GetAsync();

```