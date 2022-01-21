---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df0e02a1f3f645032c55ded33a93b4c0592dae07
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62101431"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserChat -UserId $userId -ChatId $chatId -Top 2 

```