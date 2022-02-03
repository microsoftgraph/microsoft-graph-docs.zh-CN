---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9fd6f4ddb6ec0f72e38b9945447b310b7fd66db9
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340410"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    KeyId = "f0b0b335-1d71-4883-8f98-567911bfdca6"
    Proof = "eyJ0eXAiOiJ..."
}

Remove-MgApplicationKey -ApplicationId $applicationId -BodyParameter $params

```