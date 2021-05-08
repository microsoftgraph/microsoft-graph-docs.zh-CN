---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98a1011c3f6643718b4f53d197343f277682ac46
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52240640"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewPolicy = new AccessReviewPolicy
{
    IsGroupOwnerManagementEnabled = true
};

await graphClient.Policies.AccessReviewPolicy
    .Request()
    .UpdateAsync(accessReviewPolicy);

```