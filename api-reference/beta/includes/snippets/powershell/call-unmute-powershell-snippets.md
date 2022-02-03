---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c48f11b88fb90c9a9d4079e49ebb20cd5bcd7631
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62341163"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "clientContext-value"
}

Invoke-MgUnmuteCommunicationCall -CallId $callId -BodyParameter $params

```