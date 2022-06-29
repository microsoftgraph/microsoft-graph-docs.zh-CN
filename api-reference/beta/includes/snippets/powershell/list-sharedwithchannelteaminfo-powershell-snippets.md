---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15628641ae16caa3d11af132b8110fb21f08b286
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66502300"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelSharedWithTeam -TeamId $teamId -ChannelId $channelId

```