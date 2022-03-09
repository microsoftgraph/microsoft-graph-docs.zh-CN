---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4d7ef3fbed79bebabf771753d6e9622dbb633b3c
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63393968"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserSettingContactMergeSuggestion -UserId $userId

```