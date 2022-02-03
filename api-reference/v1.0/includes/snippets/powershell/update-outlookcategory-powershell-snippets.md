---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fec9ec68e048821c0ad7cc6a3d31fa7d92627875
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349786"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Color = "preset15"
}

# A UPN can also be used as -UserId.
Update-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId -BodyParameter $params

```