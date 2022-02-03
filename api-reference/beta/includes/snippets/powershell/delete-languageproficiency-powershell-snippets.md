---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c04acd5a5a265f8a2ebb96d74e8f96231c39ee10
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352495"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Remove-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId

```