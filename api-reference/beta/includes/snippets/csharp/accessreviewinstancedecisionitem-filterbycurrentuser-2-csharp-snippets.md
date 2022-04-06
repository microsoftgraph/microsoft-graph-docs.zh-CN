---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ba930193f66039c9d4178daa10793a9723e2e43
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853426"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages["{accessReviewStage-id}"].Decisions
    .FilterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```