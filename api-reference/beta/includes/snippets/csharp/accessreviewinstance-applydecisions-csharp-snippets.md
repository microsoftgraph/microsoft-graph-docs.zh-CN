---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: de8fd723f5cbf93fbb342b652fdf50abf70151435c9b702ca8f994dcbe618470
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902686"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```