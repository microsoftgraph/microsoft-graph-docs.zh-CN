---
description: 自动生成的文件。请勿修改
ms.openlocfilehash: f325dee72c8c4197e0ffde8f3310a7c6b7ed0756
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49221896"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = await graphClient.IdentityGovernance.AccessReviews.Definitions["2b83cc42-09db-46f6-8c6e-16fec466a82d"]
    .Request()
    .GetAsync();

```