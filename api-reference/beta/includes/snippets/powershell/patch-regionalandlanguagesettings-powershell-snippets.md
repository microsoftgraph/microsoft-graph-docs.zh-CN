---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7078f613dcd883ba2030b441c3ee18dc1ba5ec05
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62102418"
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

Update-MgUserSettingRegionalAndLanguageSetting -UserId $userId -BodyParameter $params

```