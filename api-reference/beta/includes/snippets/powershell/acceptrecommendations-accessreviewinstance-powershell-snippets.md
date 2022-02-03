---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1961cddcfa20048bab4fda841020332572236eda
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340494"
---
```powershell

Import-Module Microsoft.Graph.Users.Actions

# A UPN can also be used as -UserId.
Invoke-MgAcceptUserPendingAccessReviewInstanceRecommendation -UserId $userId -AccessReviewInstanceId $accessReviewInstanceId

```