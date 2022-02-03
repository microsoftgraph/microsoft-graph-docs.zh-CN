---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6e9bf5b0e7a8cb856d5a320b8e5507f321e1db2
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62348698"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "clientContext-value"
}

Invoke-MgMuteCommunicationCall -CallId $callId -BodyParameter $params

```