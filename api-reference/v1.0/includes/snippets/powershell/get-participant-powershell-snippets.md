---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c38f686c29de98d4099e53208120607e285542b3
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097630"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Get-MgCommunicationCallParticipant -CallId $callId -ParticipantId $participantId

```