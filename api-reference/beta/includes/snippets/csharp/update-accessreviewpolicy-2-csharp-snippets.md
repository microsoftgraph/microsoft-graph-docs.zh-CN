---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 643e9de91b0b6e7750154a3c4ae8c1a42f9604c0
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240627"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = new AccessReviewPolicy
{
    IsGroupOwnerManagementEnabled = true
};

await graphClient.IdentityGovernance.AccessReviews.Policy
    .Request()
    .UpdateAsync(accessReviewPolicy);

```