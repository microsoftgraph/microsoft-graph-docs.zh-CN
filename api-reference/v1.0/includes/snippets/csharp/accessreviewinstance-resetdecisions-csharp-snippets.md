---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f2c6e4af12bb4af267abc65373b24d64ddf67164555c197f2fe769d0bfe623a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332176"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```