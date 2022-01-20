---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9ef51bb219b35fb97287aeab21fba5c8f8f54837
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62113307"
---
```powershell

Import-Module Microsoft.Graph.People

Remove-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId

```