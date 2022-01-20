---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f70d0996e1b9e6e5b89c8fcfb06e4ea1219ea143
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62124864"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageReply -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId

```