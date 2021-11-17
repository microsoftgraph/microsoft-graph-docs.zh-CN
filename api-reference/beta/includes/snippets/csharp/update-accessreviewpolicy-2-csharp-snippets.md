---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 12889a1cb3539e90058dbf9dbe81d19038f7b28c296f5c7bf96db488d30662f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902642"
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