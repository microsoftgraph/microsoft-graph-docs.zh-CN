---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1f221871a853b1f904a0a6f6ec59d29fd0deaa24
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62134272"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgTeamMember -TeamId $teamId -ConversationMemberId $conversationMemberId

```