---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 82261c2efbed6fe0de59f26b1050bf84224a2fae
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349761"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteSectionGroup -UserId $userId -SectionGroupId $sectionGroupId

```