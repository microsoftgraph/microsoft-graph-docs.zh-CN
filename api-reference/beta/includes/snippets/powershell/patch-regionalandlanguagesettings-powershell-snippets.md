---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bd1e8ce0ec5c502e63de7cda861c4c01239c5577
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351576"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    AuthoringLanguages = @(
        @{
            Locale = "en-US"
        }
        @{
            Locale = "es-MX"
        }
    )
    DefaultRegionalFormat = @{
        Locale = "en-US"
    }
}

# A UPN can also be used as -UserId.
Update-MgUserSettingRegionalAndLanguageSetting -UserId $userId -BodyParameter $params

```