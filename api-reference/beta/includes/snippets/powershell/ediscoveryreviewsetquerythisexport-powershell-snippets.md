---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6250ce2aeabb1915a926f1e70524ee455e99ebab
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442491"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    OutputName = "Export reviewset query via API"
    Description = "Export for the Contoso investigation 2"
    ExportOptions = "originalFiles,fileInfo,tags"
    ExportStructure = "directory"
}

Export-MgSecurityCaseEdiscoveryCaseReviewSetQuery -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -EdiscoveryReviewSetQueryId $ediscoveryReviewSetQueryId -BodyParameter $params

```