---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb0eabf5adacc2dba52a81c05465782464f39390
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445475"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    "Group@odata.bind" = "https://graph.microsoft.com/v1.0/groups/93f90172-fe05-43ea-83cf-ff785a40d610"
    IncludedSources = "mailbox"
}

New-MgSecurityCaseEdiscoveryCaseCustodianUnifiedGroupSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryCustodianId $ediscoveryCustodianId -BodyParameter $params

```