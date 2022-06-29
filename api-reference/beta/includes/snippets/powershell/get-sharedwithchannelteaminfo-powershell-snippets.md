---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6307d25054740eac717a36e87ae5b229aaccca6a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502756"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelSharedWithTeam -TeamId $teamId -ChannelId $channelId -SharedWithChannelTeamInfoId $sharedWithChannelTeamInfoId

```