---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0dd8ad701e32151eba513a751a8473dd5cc39331
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66446904"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    OutputName = "Export via API"
    Description = "Export for the Contoso investigation"
    ExportOptions = "originalFiles,fileInfo,tags"
    ExportStructure = "directory"
}

Export-MgSecurityCaseEdiscoveryCaseReviewSet -EdiscoveryCaseId $ediscoveryCaseId -EdiscoveryReviewSetId $ediscoveryReviewSetId -BodyParameter $params

```