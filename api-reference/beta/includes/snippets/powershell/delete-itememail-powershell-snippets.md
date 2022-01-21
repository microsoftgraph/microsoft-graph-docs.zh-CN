---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8af84732dffcf0383f476f938caa814e703dbd57
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62096363"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileEmail -UserId $userId -ItemEmailId $itemEmailId

```