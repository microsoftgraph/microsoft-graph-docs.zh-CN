---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 599acec0e5aeee2a7cbeed05f4d3598d87430c71
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62105981"
---
```powershell

Import-Module Microsoft.Graph.Mail

$params = @{
    ClassifyAs = "focused"
}

Update-MgUserInferenceClassificationOverride -UserId $userId -InferenceClassificationOverrideId $inferenceClassificationOverrideId -BodyParameter $params

```