---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 628881639dea4781053a1939e1f1ba7330c3bf25
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351962"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteSection -UserId $userId -OnenoteSectionId $onenoteSectionId

```