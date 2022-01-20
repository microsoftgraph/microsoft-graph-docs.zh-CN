---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c3cbce10f29d77472603c1083852ca2991d20442
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136037"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserUsedInsight -UserId $userId -Sort "LastUsed/LastAccessedDateTime desc" 

```