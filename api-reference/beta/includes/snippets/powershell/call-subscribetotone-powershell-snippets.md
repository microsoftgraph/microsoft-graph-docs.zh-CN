---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4130445a8a3e7c3ed298bce8b7fbdf4b7045f093
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340271"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "fd1c7836-4d84-4e24-b6aa-23188688cc54"
}

Invoke-MgSubscribeCommunicationCallToTone -CallId $callId -BodyParameter $params

```