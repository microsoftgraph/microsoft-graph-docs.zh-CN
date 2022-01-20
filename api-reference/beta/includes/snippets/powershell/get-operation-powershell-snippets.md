---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6774cb49480e9baccfca93667951d60f6dfc6013
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094906"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgUserAuthenticationOperation -UserId $userId -LongRunningOperationId $longRunningOperationId

```