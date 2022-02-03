---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 703901b596d8d5076d52c029a3129c2babb2c5d8
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352088"
---
```powershell

Import-Module Microsoft.Graph.Notes

# A UPN can also be used as -UserId.
Get-MgUserOnenoteSectionGroup -UserId $userId

```