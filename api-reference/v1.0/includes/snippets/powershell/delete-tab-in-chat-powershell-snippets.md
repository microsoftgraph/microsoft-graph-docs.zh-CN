---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 49d5a99df0d3c91decd317c512c5e4d5a8eacd98
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122316"
---
```powershell

Import-Module Microsoft.Graph.Teams

Remove-MgChatTab -ChatId $chatId -TeamsTabId $teamsTabId

```