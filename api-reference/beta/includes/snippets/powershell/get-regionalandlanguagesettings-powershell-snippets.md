---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03e34f4935887b4add2ecab51f96930199fc384b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349955"
---
```powershell

Import-Module Microsoft.Graph.Users

# A UPN can also be used as -UserId.
Get-MgUserSettingRegionalAndLanguageSetting -UserId $userId

```