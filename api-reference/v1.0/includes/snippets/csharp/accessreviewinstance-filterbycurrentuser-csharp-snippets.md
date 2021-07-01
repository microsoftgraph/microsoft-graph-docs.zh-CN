---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb8c23d3e04ff458da4680ebba827c0c08d76255
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209848"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances
    .FilterByCurrentUser(AccessReviewInstanceFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```