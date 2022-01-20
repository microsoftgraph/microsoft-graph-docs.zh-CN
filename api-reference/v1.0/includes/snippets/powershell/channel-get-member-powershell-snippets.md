---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b5eadb3c509dc42e93d00ed32c7e6dff785a188
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107655"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMember -TeamId $teamId -ChannelId $channelId -ConversationMemberId $conversationMemberId

```