---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0db40310b70c69be7ecce64f84efc466219a7a620846fec739134eab66c2f2b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .AcceptRecommendations()
    .Request()
    .PostAsync();

```