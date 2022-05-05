---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38f20e173f81de67a4dbab28041af3b0a05e9870
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65212889"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelSharedWithTeamAllowedMember -TeamId $teamId -ChannelId $channelId -SharedWithChannelTeamInfoId $sharedWithChannelTeamInfoId

```