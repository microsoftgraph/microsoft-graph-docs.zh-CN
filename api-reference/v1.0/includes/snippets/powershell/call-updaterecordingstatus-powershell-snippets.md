---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4e44b658a1b03a1c03c8ffd5efa8680da17fc267
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339039"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "clientContext-value"
    Status = "notRecording | recording | failed"
}

Update-MgCommunicationCallRecordingStatus -CallId $callId -BodyParameter $params

```