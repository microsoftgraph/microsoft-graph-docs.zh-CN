---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab3aa1a01008a0c45714df11c3015cbca62f5fdf
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442561"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Email = "AdeleV@contoso.com"
}

New-MgSecurityCaseEdiscoveryCaseCustodian -EdiscoveryCaseId $ediscoveryCaseId -BodyParameter $params

```