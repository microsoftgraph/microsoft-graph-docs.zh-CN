---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c43d8437569d83707be061104c7d2683464396c6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62342855"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamChannelEmail -TeamId $teamId -ChannelId $channelId

```