---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cf239d00bcd1600d18c715bdf1ef6bdea8f05505
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62094448"
---
```powershell

Import-Module Microsoft.Graph.Teams

Get-MgUserChat -UserId $userId -ExpandProperty "members" 

```