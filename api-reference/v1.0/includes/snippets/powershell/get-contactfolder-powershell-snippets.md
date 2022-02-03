---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1115012d02887c66c4b065922a74a905eddb4f29
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351099"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContactFolder -UserId $userId -ContactFolderId $contactFolderId

```