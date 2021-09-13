---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dd84af97a6f13839dd4505576338e1257aaddf40d8cf2c64e5fb05054a34b961
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274099"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Decisions
    .FilterByCurrentUser(AccessReviewInstanceDecisionItemFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```