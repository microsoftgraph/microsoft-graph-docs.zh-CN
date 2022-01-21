---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a72345742fb0ad63a818948a285aa69d24c52a9a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62132830"
---
```powershell

Import-Module Microsoft.Graph.People

$params = @{
    DisplayName = "Norwegian Bokmål"
    Tag = "nb-NO"
    Spoken = "nativeOrBilingual"
    Written = "nativeOrBilingual"
    Reading = "nativeOrBilingual"
}

New-MgUserProfileLanguage -UserId $userId -BodyParameter $params

```