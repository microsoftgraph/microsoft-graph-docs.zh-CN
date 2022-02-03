---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3f4fbea0c5877fb4d1fb45d21d87a6fc374902e
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352260"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfileAddress -UserId $userId

```