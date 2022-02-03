---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb6349fe047b0b4d2886f797de3e96403e820bfa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351167"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePublication -UserId $userId -ItemPublicationId $itemPublicationId

```