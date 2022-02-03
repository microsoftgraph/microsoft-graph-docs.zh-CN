---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b54f1ee84c12eeeed2e533d285a4a796f6cc10cf
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340492"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

$params = @{
    Decision = "Approve"
    Justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team"
    ResourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}

# A UPN can also be used as -UserId.
Invoke-MgBatchUserPendingAccessReviewInstanceRecordDecision -UserId $userId -AccessReviewInstanceId $accessReviewInstanceId -BodyParameter $params

```