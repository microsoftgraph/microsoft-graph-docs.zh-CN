---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fb975f88b6a6f8640f76da6de0f90a5825a129be
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446721"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Site = @{
        WebUrl = "https://m365x809305.sharepoint.com/sites/Retail"
    }
}

New-MgSecurityCaseEdiscoveryCaseLegalHoldSiteSource -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryHoldPolicyId $ediscoveryHoldPolicyId -BodyParameter $params

```