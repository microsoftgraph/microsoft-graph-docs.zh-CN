---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66344f76ca269f3d8b8b525fcb87c1a3fb9eb224
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350300"
---
```powershell

Import-Module Microsoft.Graph.People

# A UPN can also be used as -UserId.
Get-MgUserPerson -UserId $userId

```