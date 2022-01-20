---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65e016cb9e635ae9dece620b9847ad53413c9166
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62129743"
---
```powershell

Import-Module Microsoft.Graph.People

Get-MgUserProfileLanguage -UserId $userId -LanguageProficiencyId $languageProficiencyId

```