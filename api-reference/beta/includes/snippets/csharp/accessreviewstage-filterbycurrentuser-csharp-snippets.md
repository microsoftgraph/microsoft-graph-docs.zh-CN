---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 53087000571c7e4651638e795a671baa46e70074
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854150"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages
    .FilterByCurrentUser(AccessReviewStageFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```