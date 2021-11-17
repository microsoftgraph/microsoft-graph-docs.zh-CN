---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a726b9c130b611ea1aa35e2ea97e5f501a1b042f2dc33950573ac97583b9f14c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .Stop()
    .Request()
    .PostAsync();

```