---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9306ae08b539c4f0367317b99091558c9c8001ba
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100641"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserChat -UserId $userId -ChatId $chatId

```