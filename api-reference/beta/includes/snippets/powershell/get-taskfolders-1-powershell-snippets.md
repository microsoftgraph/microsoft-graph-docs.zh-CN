---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 38e6b796bf4195a0ae4cfa7110fcc90b69aaa775
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62135370"
---
```powershell

Import-Module Microsoft.Graph.Users

Get-MgUserOutlookTaskGroupTaskFolder -UserId $userId -OutlookTaskGroupId $outlookTaskGroupId

```