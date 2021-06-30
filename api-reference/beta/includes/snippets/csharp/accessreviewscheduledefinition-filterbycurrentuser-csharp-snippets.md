---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3f1f97bb845cd977edd91b4e9731734f48f77df
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207398"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .FilterByCurrentUser(AccessReviewScheduleDefinitionFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```