---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 512354997cab7577330d4e7f1b211ab180944d9b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122379"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId -ConversationMemberId $conversationMemberId

```