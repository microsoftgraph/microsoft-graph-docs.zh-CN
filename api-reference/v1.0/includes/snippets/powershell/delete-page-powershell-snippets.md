---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a0f1e9902ea5f1d30b03e5051652238243e4f3c6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350006"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Remove-MgUserOnenotePage -UserId $userId -OnenotePageId $onenotePageId

```