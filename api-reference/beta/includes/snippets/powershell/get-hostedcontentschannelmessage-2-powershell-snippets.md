---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e2086cbceb282f9a95462f8e8e0549726860e97
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66441971"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamChannelMessageReplyHostedContent -TeamId $teamId -ChannelId $channelId -ChatMessageId $chatMessageId -ChatMessageId1 $chatMessageId1

```