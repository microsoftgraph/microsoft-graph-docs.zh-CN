---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e3ba8870b0ef05fb975527936f507a468277d225
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129511"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

Get-MgRiskyUserHistory -RiskyUserId $riskyUserId -RiskyUserHistoryItemId $riskyUserHistoryItemId

```