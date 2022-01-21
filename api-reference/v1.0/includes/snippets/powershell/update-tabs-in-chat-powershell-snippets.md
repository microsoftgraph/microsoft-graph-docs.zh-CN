---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f1d990d3bd3179936796726186e2c577e71201c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62107627"
---
```powershell

Import-Module Microsoft.Graph.Teams

$params = @{
    DisplayName = "My Contoso Tab - updated again"
}

Update-MgChatTab -ChatId $chatId -TeamsTabId $teamsTabId -BodyParameter $params

```