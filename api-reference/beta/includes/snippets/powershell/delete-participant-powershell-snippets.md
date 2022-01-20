---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 26c6ee3554ecca25b53fe81fa023d435a802c316
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133208"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Remove-MgCommunicationCallParticipant -CallId $callId -ParticipantId $participantId

```