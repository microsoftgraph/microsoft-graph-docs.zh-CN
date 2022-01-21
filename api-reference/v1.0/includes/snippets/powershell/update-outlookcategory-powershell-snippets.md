---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eba45d50d8120e776254825530716f4246d776e2
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62092162"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    Color = "preset15"
}

Update-MgUserOutlookMasterCategory -UserId $userId -OutlookCategoryId $outlookCategoryId -BodyParameter $params

```