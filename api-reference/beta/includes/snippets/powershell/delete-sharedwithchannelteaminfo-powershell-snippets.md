---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69aa45ec40e7e4b5cbd2627c065a69cba0b84699
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502430"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamChannelSharedWithTeam -TeamId $teamId -ChannelId $channelId -SharedWithChannelTeamInfoId $sharedWithChannelTeamInfoId

```