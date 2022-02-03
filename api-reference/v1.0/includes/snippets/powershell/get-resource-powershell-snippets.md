---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3071be91fbb45ac810859bd129726ef62f4cdcd3
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351677"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteResourceContent -UserId $userId -OnenoteResourceId $onenoteResourceId

```