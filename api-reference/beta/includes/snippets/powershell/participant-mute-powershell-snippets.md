---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9c46b32668836298722c909eb60654787e18f8a9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502266"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    ClientContext = "d45324c1-fcb5-430a-902c-f20af696537c"
}

Invoke-MgMuteCommunicationCallParticipant -CallId $callId -ParticipantId $participantId -BodyParameter $params

```