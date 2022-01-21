---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2b2c992920690f95bf7d050fc491387a7574aed
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107696"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamChannel -TeamId $teamId -ChannelId $channelId

```