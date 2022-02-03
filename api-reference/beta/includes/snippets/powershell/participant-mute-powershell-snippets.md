---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bc0bdf7b4d7b10b48fb8390c79bd4cc7c3f197fc
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346114"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
}

Invoke-MgMuteAllCommunicationCallParticipant -CallId $callId -ParticipantId $participantId -BodyParameter $params

```