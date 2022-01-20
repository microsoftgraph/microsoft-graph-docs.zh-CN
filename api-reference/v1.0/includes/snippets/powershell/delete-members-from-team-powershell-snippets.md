---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27012b635706303c666b8dbbacc4bb497211e64c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62087801"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgTeamMember -TeamId $teamId -ConversationMemberId $conversationMemberId

```