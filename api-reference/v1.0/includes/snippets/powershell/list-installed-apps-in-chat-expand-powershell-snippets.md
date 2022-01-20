---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c1130ee8a42873c0ef4243d795acb91224c3139
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088839"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgChatInstalledApp -ChatId $chatId -ExpandProperty "teamsAppDefinition(`$expand=bot)" 

```