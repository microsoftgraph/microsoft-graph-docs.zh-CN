---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: feb65cc82f1bba6994911498b32b6bffce524565
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440432"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    DisplayName = "My Query 1"
    ContentQuery = "(Author="edison")"
}

New-MgSecurityCaseEdiscoveryCaseReviewSetQuery -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -BodyParameter $params

```