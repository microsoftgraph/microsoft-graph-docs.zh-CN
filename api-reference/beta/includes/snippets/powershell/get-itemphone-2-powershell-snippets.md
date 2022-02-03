---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ff6a7d55e12051097e133d7cc11b241f618d018
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351861"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserProfilePhone -UserId $userId

```