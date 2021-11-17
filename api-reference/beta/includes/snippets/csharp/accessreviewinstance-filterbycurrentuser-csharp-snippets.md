---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1aaa04f76c314652edd9f4166f2702367fa4f42fec8a9668fab8e947ef063851
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances
    .FilterByCurrentUser(AccessReviewInstanceFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```