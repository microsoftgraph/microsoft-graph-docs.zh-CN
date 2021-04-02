---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93755ff9f3cf850a4322a90ebaee97e193f68d03
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507479"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decision = "Approve";

var justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team";

var resourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a";

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"]
    .BatchRecordDecisions(decision,justification,null,resourceId)
    .Request()
    .PostAsync();

```