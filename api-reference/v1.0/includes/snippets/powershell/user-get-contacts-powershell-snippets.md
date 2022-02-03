---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd5e4d912591f5e1ef615f0d1a98e107675bf105
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350864"
---
```powershell

Import-Module Microsoft.Graph.PersonalContacts

# A UPN can also be used as -UserId.
Get-MgUserContact -UserId $userId

```