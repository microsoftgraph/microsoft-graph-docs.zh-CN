---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99c0f916af7da092429d229d5157a8b91e5d180c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62114293"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

Remove-MgCommunicationCallAudioRoutingGroup -CallId $callId -AudioRoutingGroupId $audioRoutingGroupId

```