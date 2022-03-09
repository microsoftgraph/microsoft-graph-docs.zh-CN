---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ab933c7a9a63280aafa8a3efccf0fdd03d170f96
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395102"
---
```powershell

Import-Module Microsoft.Graph.Users

$params = @{
    IsEnabled = $false
}

# A UPN can also be used as -UserId.
Update-MgUserSettingContactMergeSuggestion -UserId $userId -BodyParameter $params

```